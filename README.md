# Chess-Engine

![Sample of image of game](https://github.com/JaehyeongPark06/Chess-Engine/assets/78674944/fecfd2be-8e9b-4972-9cc8-ed28f8b48456)

https://github.com/JaehyeongPark06/Chess-Engine/assets/78674944/c243ebcc-5666-4394-8f55-f98df71b6346

## About

A chess engine using the Negamax algorithm and other optimization techniques able to consistently beat the 2200 rated bot on chess.com (Noam).
The GUI includes undoing moves, flipping and resetting the board, under promotions, and custom board positions and evaluation times.

## Libraries and Tools Used

- [Bootstrap](https://getbootstrap.com/) for GUI buttons.

## Algorithms and Optimization Techniques Used

- Negamax algorithm simplifies the implementation of the minimax algorithm by taking advantage of the zero-sum nature of the game.
- Alpha-beta pruning refines the search by eliminating branches that are guaranteed not to affect the final decision.
- Iterative deepening explores the most promising moves first, making the best use of the available search time.
- Piece-square tables evaluates the relative value of pieces on the board, guiding the search algorithm towards better moves.
- Move ordering using the MVV-LVA heuristic prioritizes moves that capture high-value pieces and also reduces the search space.
- Principal variation search improves the efficiency of the search process by searching only the most promising lines of play.
- Quiescence search ensures that the evaluation of the position is stable by extending the search to positions where there are no - captures or checks.
- Zobrist hashing stores the game state in a compact and efficient way, allowing for quick comparisons and detection of repetitions.
- Late move reduction optimies the search process by reducing the depth of the search for moves that are considered less promising.
- Mate distance pruning cuts trees and adjust bounds of lines where no shorter mate is possible
- Null move pruning (Null Move Heuristic, NMH) reduces the search space by seeing if a null move (a move that passes the turn back to the opponent), still results in a position that is better than the alpha threshold. If it is a better position, then actual moves are likely to result in an even better position.

## Possible Improvements

- Switching programming languages
- Using a more detailed evaluation method (ex. use of opening tables)
- Transposition Tables
- Replacing the [Simplified Evaluation Function](https://www.chessprogramming.org/Simplified_Evaluation_Function) with [PeSTO's Evaluation Function](https://www.chessprogramming.org/PeSTO%27s_Evaluation_Function)

## License

See [License](https://github.com/JaehyeongPark06/Chess-Engine/blob/main/LICENSE)

#### You can play against it [here](https://chess.jadenpark.ca)
