## 概述

这个一个简易版快速接入[涂鸦的小程序 SDK](https://developer.tuya.com/cn/docs/iot/app-development/mini-programs/overview/applet-ecology?id=K9ptacgp94o5d)，[配网插件](https://developer.tuya.com/cn/docs/iot/app-development/mini-programs/tuya-applet-with-web-plugin/distribution-network-plugin?id=K9lq218xn0wn8) 和 MQTT 的连接的Demo，目前趋于稳定。后续还会有新功能的更新。

## 体验

如果需要在自己的小程序中嵌入小程序配网的功能，可以通过接入小程序 SDK，获取自己的票据信息，然后调用小程序插件，完成配网，配网成功后重新调用获取设备信息的接口即可。

如果需要在自己的小程序中开发设备控制，场景联动、自动化等功能，可以通过小程序 SDK 调用相应的接口即可。

如果需要涂鸦公版小程序来支持您的设备，可以联系我们。公版小程序的您可以扫码下面的二维码体验：

<p align="center">
<img width=200 src="https://images.tuyacn.com/rms-static/9cbc9210-cb1f-11ea-9723-5fcc4b1eeb4e-1595314722225.jpg?tyName=gh_42ad2888c42d_258.jpg" >
</p>

## 文件介绍

```
├── components             // 组件库
├── image                  // 图片库
├── libs                   // 第三方库
├── pages                  // 具体页面的目录
├── utils                  // 基础工具库
├── app.js                 // 小程序入口
├── app.json               // 小程序全局配置文件
├── project.config.json    // 项目配置文件
└── README.md              // 说明文件
```

## Demo 说明

- 设备配网：

  直接点击按钮进行配网：目前支持 AP 配网、扫码配网、蓝牙配网、zigbee 配网

- 体验设备功能：

  添加设备完成后，可以点击设备开启开关进行设备 MQTT 消息推送调试，建议先使用 api.js 文件中的 getDeviceSpecifications 函数获取指令集，防止出现 dp 点字段名称可能不一致的情况。正常下发指令后页面上会显示出推送消息的内容

- 完整版Demo
  目前支持设备控制，消息推送，添加设备(配网), 家庭模块

## 视频演示
哔哩哔哩视频：https://www.bilibili.com/video/BV1vL411H7Ph

<video id="video" controls="" preload="none" poster="封面">
      <source id="mp4" src="https://www.bilibili.com/video/BV1vL411H7Ph?share_source=copy_web" type="video/mp4">
</videos>
