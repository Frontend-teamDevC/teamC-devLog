``` mermaid
classDiagram

class Table {
  <<Abstract>>
  - gameType: string
  - betDenominations: number[]
  - turnCounter: number = 0
  - gamePhase: string = 'betting'
  - resultsLog: string[]
  - deck: Deck
  - players: Player[]
  - dealer: Player

  constructor 
  + Table(gameType: string, betDenominations: number[])

  + assignPlayerHands()void
  + clearPlayerHandsAndBets()void  
  + onLastPlayer()boolean
  + onFirstPlayer()boolean

  Abstract + evaluateAndGetRoundResults() string
  Abstract + evaluateMove(player: Player) void
  Abstract + getTurnPlayer(): Player
  Abstract + haveTurn(userData: number) void
}

class PokerTable {   
  + getHandScore() number
  + getDeler() number
}

class Player {
  <<abstract>>
  - name: string
  - type: string
  - gameType: string
  - chips: number
  - bet: number = 0
  - winAmount: number = 0
  - gameStatus: string = 'betting'
  - hand: Card[]
  constructor + Player(name: string, type: string, gameType: string, chips: number = 400)
  
  abstract + promptPlayer(userData: number | null) GameDecision
  abstract + getHandScore() number
}

class PokerPlayer {
  + promptPlayer(userData: number | null) GameDecision
  + getHandScore() number
}


class GameDecision {
  - action: string
  - amount: number
  <<constructor>> + GameDecision(action: string, amount: number)
}


class Deck {
  - gameType: string
  - cards: Card[]
  <<constructor>>
  + Deck(gameType: string)
  + shuffle() void
  + resetDeck(gameType: string) Card[]
  + drawCard() Card
}

class Card {
  - suit: string
  - rank: string
  <<constructor>>
  + Card(suit: string, rank: string)
  + getRankNumber(sum: number) number
}

Table <|-- PokerTable : extends

Player <|-- PokerPlayer : extends

PokerTable "1" --> "1..*" PokerPlayer : contains
PokerTable "1" --> "1" Deck : contains
PokerPlayer --|> GameDecision : creates

Deck --> Card : owns

```