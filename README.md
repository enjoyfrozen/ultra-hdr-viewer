# Ultra HDR Meta Data viewer

20240827
Version: V1.0
1. 支持GrayScale Gainmap 或者 ColorScale GainMap
即兼容支持苹果或者Android设备拍摄的HDR JPEG。


 https://developer.android.com/media/platform/hdr-image-format
 https://developer.adobe.com/xmp/docs/XMPNamespaces/exif/
 https://github.com/adobe/XMP-Toolkit-SDK/blob/main/docs/XMPSpecificationPart3.pdf
 https://helpx.adobe.com/content/dam/help/en/camera-raw/using/gain-map/jcr_content/root/content/flex/items/position/position-par/table/row-io13dug-column-4a63daf/download_section/download-1/gain_map_demo_appdocs1.pdf

关于ColorScale GainMap与GrayScale GainMap的兼容性： 
 从HDR显示的角度来说，其实效果应该是一样的，但如果是从映射的角度，color gain map无疑会更好，但体积也相应会增加两到三倍。
 
1.苹果全系，三星s24 ultra、pixel7/8、一加12海外版等其他已适配安卓手机，无论是原生相机拍摄还是相册显示，都只支持grayscale gain map.

2.instagram 目前只支持grayscale gain map。

3.Adobe系(ACR和lightroom）导出的为 color gain map，pixelmator和photomator导出的为 grayscale gain map。

4.谷歌相册移动端以及Gain map Demo App两者都支持正常显示，且HDR效果完全一样，chromium核心的浏览器也是两者都支持，但亮度略有不同，color gain map为正常亮度，grayscale gain map则略暗1至2档。

refers:
关于Ultra HDR Image的那些事
https://blog.csdn.net/feelabclihu/article/details/134473423

![image](https://github.com/enjoyfrozen/ultra-hdr-viewer/blob/main/android_hdr_generate.png)


HDR照片初步探究
https://sspai.com/post/87316