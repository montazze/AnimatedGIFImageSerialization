AnimatedGIFImageSerialization
=============================

`AnimatedGIFImageSerialization` decodes an `UIImage` from [Animated GIFs](http://en.wikipedia.org/wiki/Graphics_Interchange_Format) image data, following the API conventions of Foundation's `NSJSONSerialization` class.

Out of the box, `UIImage` does not support decoding animated gifs into an animated `UIImage`. So long as `ANIMATED_GIF_NO_UIIMAGE_INITIALIZER_SWIZZLING` is not `#define`'d, the this library will swizzle the `UIImage` initializers to support animated GIFs.

## Usage

### Decoding

```objective-c
UIImageView *imageView = ...;
imageView.image = [UIImage imageNamed:@"animated.gif"];
```

![Animated GIF](https://raw.githubusercontent.com/mattt/AnimatedGIFImageSerialization/master/Example/Animated%20GIF%20Example/animated.gif)

---

## Contact

Mattt Thompson

- http://github.com/mattt
- http://twitter.com/mattt
- m@mattt.me

## License

AnimatedGIFImageSerialization is available under the MIT license. See the LICENSE file for more info.
