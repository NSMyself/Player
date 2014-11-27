## Player

`Player` is a simple iOS video player written in [Swift](https://developer.apple.com/swift/).

It provides a quick means to play local or stream remote media, but also enables easy customization of loading and user interaction.

If you're looking for a video player written in Objective-C, checkout [PBJVideoPlayer](https://github.com/piemonte/PBJVideoPlayer).

Please review the [release history](https://github.com/piemonte/player/releases) for more information.

[![Build Status](https://travis-ci.org/piemonte/player.svg)](https://travis-ci.org/piemonte/player)

## Installation

Once [CocoaPods](http://cocoapods.org/) starts [supporting Clang Modules / Frameworks](https://github.com/CocoaPods/CocoaPods/issues/2272), I hope to distribute `Player` by that means. Until then, just copy the `Player.swift` file into your Xcode project.

## Usage

The sample project provides an example of how to integrate `Player`, otherwise you can follow these steps.

Allocate and add the `Player` controller to your view hierarchy.

``` Swift
 self.player = Player()
 self.player.delegate = self
 self.player.view.frame = self.view.bounds
    
 self.addChildViewController(self.player)
 self.view.addSubview(self.player.view)
 self.player.didMoveToParentViewController(self)
```

Provide the file path to the resource you would like to play locally or stream. Ensure you're including the file extension.

``` Swift
 self.player.path = "Video.mp4"
```

play/pause/chill

``` Swift
 self.player.playFromBeginning()
```

## Community

- Need help? Use [Stack Overflow](http://stackoverflow.com/questions/tagged/player-swift) with the tag 'player-swift'.
- Questions? Use [Stack Overflow](http://stackoverflow.com/questions/tagged/player-swift) with the tag 'player-swift'.
- Found a bug? Open an [issue](https://github.com/piemonte/player/issues).
- Feature idea? Open an [issue](https://github.com/piemonte/player/issues).
- Want to contribute? Submit a [pull request](https://github.com/piemonte/player/pulls).

## Resources

* [AV Foundation Programming Guide](https://developer.apple.com/library/ios/documentation/AudioVideo/Conceptual/AVFoundationPG/Articles/00_Introduction.html)
* [PBJVision, iOS camera engine, features touch-to-record video, slow motion video, and photo capture](https://github.com/piemonte/PBJVision)
* [PBJVideoPlayer, a simple iOS video player in Objective-C](https://github.com/piemonte/PBJVideoPlayer)
* [objc.io Issue #16, Swift](http://www.objc.io/issue-16/)

## License

Player is available under the MIT license, see the [LICENSE](https://github.com/piemonte/player/blob/master/LICENSE) file for more information.

