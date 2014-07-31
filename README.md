## Swiftris: Build Your First iOS Game With Swift

<center>![](https://d1rn32hddkla48.cloudfront.net/assets/books/swiftris/whatyoubuild-b21c6fc044aa028515f362037954068a.gif)</center>

This repository maintains the completed source code indicative of the project you may build yourself by completing the [Swiftris Bloc Book](https://www.bloc.io/swiftris-build-your-first-ios-game-with-swift). Swiftris is a Tetris clone written entirely in **Swift** which employs **SpriteKit**. The organization of this project is as follows:

| **File** | **Purpose** | **Layer** |
| :---: | --- | :---: |
| `Array2D.swift` | A custom Array class which supports a `[column, row]` subscript for accessing a grid | Logic |
| `Block.swift` | Defines and represents a single square tile on the game board via column, row and color references | Logic |
| `Shape.swift` | A base class which may represent a Tetromino. This class arranges four `Block` objects in an order defined by its subclasses. It also manages rotation, | Logic |
| `SquareShape.swift` | A subclass of `Shape` which specifies the placement and rotation of the **O** Tetromino | Logic |
| `LineShape.swift` | A subclass of `Shape` which specifies the placement and rotation of the **Line** Tetromino | Logic |
| `SShape.swift` | A subclass of `Shape` which specifies the placement and rotation of the **S** Tetromino | Logic |
| `ZShape.swift` | A subclass of `Shape` which specifies the placement and rotation of the **Z** Tetromino | Logic |
| `LShape.swift` | A subclass of `Shape` which specifies the placement and rotation of the **L** Tetromino | Logic |
| `JShape.swift` | A subclass of `Shape` which specifies the placement and rotation of the **J** Tetromino | Logic |
| `TShape.swift` | A subclass of `Shape` which specifies the placement and rotation of the **T** Tetromino | Logic |
| `Swiftris.swift` | This class maintains the game logic. It generates all shapes and tracks level and score | Logic |
| `GameViewController.swift` | The single View Controller responsible for bridging the gap between the `Swiftris` and `GameScene` objects. It also responds to several gestures: swipe, pan and tap. Lastly, it updates the score and level labels | User Interface |
| `GameScene.swift` | A subclass of `SKScene` which is responsible for drawing, redrawing and animating all blocks to and from the game board. It also is responsible for sound playback | Visual |
| `Main.storyboard` | The storyboard provides the view for `GameViewController` in which the score and level labels are defined | Visual |

## Bloc
If you enjoyed Swiftris and would like to read more Bloc Books, check out [Jottly.](https://www.bloc.io/build-your-first-website-with-html-and-css) Bloc's Jottly book teaches you how to build your very first website using HTML, CSS and the Skeleton framework.
