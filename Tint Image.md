# Quartz


[https://gist.github.com/Shilo/1292152](https://gist.github.com/Shilo/1292152)

如何使用CGImageCreateWithMaskingColors去除image内的指定color

[http://stackoverflow.com/a/7377827/1391851](http://stackoverflow.com/a/7377827/1391851)

Tint PNG image
```
UIGraphicsBeginImageContextWithOptions (myIconImage.size, NO, [[UIScreen mainScreen] scale]); // for correct resolution on retina, thanks @MobileVet
CGContextRef context = UIGraphicsGetCurrentContext();

CGContextTranslateCTM(context, 0, myIconImage.size.height);
CGContextScaleCTM(context, 1.0, -1.0);

CGRect rect = CGRectMake(0, 0, myIconImage.size.width, myIconImage.size.height);

// image drawing code here

UIImage *coloredImage = UIGraphicsGetImageFromCurrentImageContext();
UIGraphicsEndImageContext();
```

[http://iosdevelopertips.com/graphics/convert-an-image-uiimage-to-grayscale.html](http://iosdevelopertips.com/graphics/convert-an-image-uiimage-to-grayscale.html)

Convert an Image (UIImage) to Grayscale

[http://nscookbook.com/2013/05/ios-programming-recipe-24-creating-a-mask-for-clipping-drawings/](http://nscookbook.com/2013/05/ios-programming-recipe-24-creating-a-mask-for-clipping-drawings/)

使用Mask

