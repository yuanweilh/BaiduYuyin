### 注意
### 因为Player的依赖库对Nodejs 4.0支持不好，请不要随意升级到新版本
## 如果你是Mac用户的话，我已经使用本地播放器来播放语音文件了，不过话说回来，如果是Mac的话本身就有语音库了

Baidu Yuyin 百度语音合成
-----------------------

使用Baidu的在线语音合成服务，需要自己申请API Key，申请网址http://yuyin.baidu.com

更新1.0.1[2015-9-18]
----------------------
1. Mac用户现在使用本地播放器来播放语音文件

更新1.0.2[2015-9-19]
----------------------
1. 使用绝对地址保存零时语音文件

跟新1.0.3[2016-7-21]
----------------------
1. 增加了缓存sessionToken到本地的功能，免得每次都去请求一边，超过24小时重新请求
2. Linux系统使用mplayer命令播放语音文件,请自行安装哦
3. 自动删除下载的mp3文件

使用方法
-------
### 安装

npm install baidu_yuyin

### 使用
```javascript
var BDSpeech = require("BDSpeech");
var speech = new BDSpeech(apiKey, secretKey);
speech.speak("你好世界")
```
