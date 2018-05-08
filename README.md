# iPhone 设备信息列表
### iOS `开发需要知道的`


### 期望大家共同书写市场调研结果


#### iOS 获取设备名

```objc
    //导入系统库
    #import <sys/utsname.h> // struct utsname systemInfo;
    
    //获取 设备名（device_name）
    - (NSString*) getDeviceName
    {
        struct utsname systemInfo;
        uname(&systemInfo);
        return  [NSString stringWithCString:systemInfo.machine
        encoding:NSUTF8StringEncoding];
    }
```

-


iOS device_name 列表说明
======================

iphone 后面 字母意思:
------------------
- S->代表speed（速度）
- C->既代表的是“Cheap”也代表的是“Color”
- plus->更大版本，极限版本

iphone列表
---------

|   机型  |device_name| 特殊描述 |   年份   |
|--------|:--------:| --------:|--------:|
|iphone4 |iPhone3,1 |  不支持3G |  2010   |
|iphone4 |iPhone3,2 |  不支持3G |  2010   |
|iphone4s|iPhone4,1 | 有电信版本 |  2010   |
|iphone5 |iPhone5,1 | 4G网络功能 |  2011   |
|iphone5 (GSM+CDMA) |iPhone5,2 | 已宣布停产 |  2011   |
|iphone5c|iPhone5,3 |苹果推出的带有合约版本|  2013   |
|iphone5c (GSM+CDMA) |iPhone5,4 |苹果推出的带有合约版本|  2013   |
|iphone5s CDMA|iPhone6,1 | Touch ID |  2013   |
|iphone5s (GSM+CDMA)|iPhone6,2 | Touch ID |  2013   |
|iphone6 |iPhone7,1 | Touch ID |  2014   |
|iphone6 plus|iPhone7,2 | Touch ID |  2014   |
|iphone6s |iPhone8,1 | 3DTouch |  2015   |
|iphone6s plus |iPhone8,2 | 3DTouch |  2015   |
|iPhone SE | iPhone8,4 |   |     |
|iphone7 |iPhone9,1 |          |  2016   |
|iphone7 |iPhone9,3 |          |  2016 美版、台版iPhone 7 |
|iphone7 plus |iPhone9,2 |          |  2016 港行、国行iPhone 7 Plus  |
|iphone7 plus |iPhone9,4 |          |  2016 美版、台版iPhone 7 Plus   |
|iphone8 |iPhone10,1 |          |  北京时间2017年9月13日凌晨1点 国行(A1863)、日行(A1906)iPhone 8  |
|iphone8 |iPhone10,2 |          |  美版(Global/A1905)iPhone 8 |
|iphone8 plus |iPhone10,2 |          |  2017 国行(A1864)、日行(A1898)iPhone 8 Plus  |
|iphone8 plus |iPhone10,5 |          | 美版(Global/A1897)iPhone 8 Plus|
|iphoneX |iPhone10,3 |          |  2017 国行(A1865)、日行(A1902)iPhone X   |
|iphoneX |iPhone10,6 |          |  2017 美版(Global/A1901)iPhone X   |


iPod Touch列表
-------------

|   机型  |device_name| 特殊描述  |   年份   |
|--------|:--------:| --------:|--------:|
| iPod1  | iPod1,1  |          |2002.3.21|
| iPod2  | iPod2,1  |          |2002.6.17|
| iPod3  | iPod3,1  |          |2003.4.28|
| iPod4  | iPod4,1  |          |2004.7.19|
| iPod5  | iPod5,1  |          |  2004   |


iPad列表
-------

|   机型  |device_name| 特殊描述  |   年份   |
|--------|:--------:| --------:|--------:|
| iPad1  | iPad1,1  |   已停产  |  2010   |
| iPad1 3G | iPad1,2  |   已停产  |     |
| iPad2 (WiFi) | iPad2,1  |          |  2011   |
| iPad2  | iPad2,2  |          |  2011   |
| iPad2  (CDMA) | iPad2,3  |          |  2011   |
| iPad2  | iPad2,4  |          |  2011   |
|iPad Mini (WiFi)| iPad2,5  |          |  2012   |
|iPad Mini2| iPad2,6  |          |  2013   |
|iPad Mini3 (GSM+CDMA) | iPad2,7  |          |  2014   |
|iPad Mini4| iPad2,8  |          |  2015   |
| iPad3 (WiFi) | iPad3,1  |          |  2012   |
| iPad3 (GSM+CDMA) | iPad3,2  |          |  2007   |
| iPad3  | iPad3,3  |          |  2007   |
| iPad4  (WiFi) | iPad3,4  |          |     |
| iPad4  | iPad3,5  |          |     |
| iPad4 (GSM+CDMA) | iPad3,6  |          |      |
| iPad Air (WiFi) | iPad4,1  |          |      |
| iPad Air (Cellular) | iPad4,2  |          |      |
| iPad Mini 2 (WiFi) | iPad4,4  |          |      |
| iPad Mini 2 (Cellular) | iPad4,5  |          |      |
| iPad Mini 2 | iPad4,6  |          |      |
| iPad Mini 3 | iPad4,7  |          |      |
| iPad Mini 3 | iPad4,8  |          |      |
| iPad Mini 3 | iPad4,9  |          |      |
| iPad Mini 4 (WiFi) | iPad5,1  |          |      |
| iPad Mini 4 (LTE) | iPad5,2  |          |      |
| iPad Air 2 | iPad5,3  |          |      |
| iPad Air 2 | iPad5,4  |          |      |
| iPad Pro 9.7 | iPad6,3  |          |      |
| iPad Pro 9.7 | iPad6,4  |          |      |
| iPad Pro 12.9 | iPad6,7  |          |      |
| iPad Pro 12.9 | iPad6,8  |          |      |
| iPad 5 (WiFi) | iPad6,11  |          |      |
| iPad Pro 12.9 inch 2nd gen (WiFi) | iPad7,1  |          |      |
| iPad Pro 12.9 inch 2nd gen (Cellular) | iPad7,2  |          |      |
| iPad Pro 10.5 inch (WiFi) | iPad7,3  |          |      |


Apple TV 列表
-------

|   机型  |device_name| 特殊描述  |   年份   |
|--------|:--------:| --------:|--------:|
| Apple TV 2  | AppleTV2,1  |     |     |
| Apple TV 3  | AppleTV3,1  |     |     |
| Apple TV 3  | AppleTV3,2  |     |     |
| Apple TV 4  | AppleTV5,3  |     |     |


如果你有想说的可以 [issues I](https://github.com/srxboys/iphoneDevice_List/issues) 。
:sweat_smile::sweat_smile::sweat_smile::sweat_smile::sweat_smile:
