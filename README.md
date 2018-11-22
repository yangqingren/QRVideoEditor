# QRVideoEditor

[![CI Status](https://img.shields.io/travis/yangqingren/QRVideoEditor.svg?style=flat)](https://travis-ci.org/yangqingren/QRVideoEditor)
[![Version](https://img.shields.io/cocoapods/v/QRVideoEditor.svg?style=flat)](https://cocoapods.org/pods/QRVideoEditor)
[![License](https://img.shields.io/cocoapods/l/QRVideoEditor.svg?style=flat)](https://cocoapods.org/pods/QRVideoEditor)
[![Platform](https://img.shields.io/cocoapods/p/QRVideoEditor.svg?style=flat)](https://cocoapods.org/pods/QRVideoEditor)

## Example

To run the example project, clone the repo, and run `pod install` from the Example directory first.

## Requirements


    /**
     timeRange

     * @param url video path
     * @param startTime
     CMTimeMakeWithSeconds(0, videoAsset.duration.timescale);

     * @param endTime
     * CMTimeMake(a,b)
     CMTimeMakeWithSeconds(a,b)

     * @param fileName video name .mp4
     * @param completion urlPath

     * If you need clipping video clips, then insert startTime and endTime to intercept the video.The parameters of video interception should be noted in CMTime format.
     */
    + (void)videoEditByTimeRangeWithUrl:(NSURL *)url startTime:(CMTime)startTime endTime:(CMTime)endTime fileName:(NSString *)fileName completion:(void (^)(NSString *urlPath))completion;

    /**
     expression or watermark

     * @param url video path
     * @param image The expression and watermark you need to add
     * @param frame The expression you need to add and the location of the watermark.
     * @param fileName video name .mp4
     * @param completion urlPath
     */
    + (void)videoEditByImageWithUrl:(NSURL *)url image:(UIImage *)image frame:(CGRect)frame fileName:(NSString *)fileName completion:(void (^)(NSString *urlPath))completion;

    /**
     text or barrage

     * @param url video path
     * @param textLayer The text or barrage you need to add
     * @param frame The text you need to add and the location of the watermark.
     * @param fileName video name .mp4
     * @param completion urlPath
     */
    + (void)videoEditByTextWithUrl:(NSURL *)url textLayer:(CATextLayer *)textLayer frame:(CGRect)frame fileName:(NSString *)fileName completion:(void (^)(NSString *urlPath))completion;

## Installation

QRVideoEditor is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'QRVideoEditor'
```

## Author

yangqingren, 564008993@qq.com

## License

QRVideoEditor is available under the MIT license. See the LICENSE file for more info.
