## PLDroidMediaStreaming 简介

`PLMediaStreamingKit` 提供两个层次的 API

PLStreamingKit 提供包括音视频编码，封包以及网络发送功能，`PLCameraStreamingKit` 除了提供 `PLStreamingKit` 的功能以外还提供了内置的采集，音视频处理以及一些系统打断事件的处理等。我们强烈推荐对音视频没有太多了解的开发者使用 `PLCameraStreamingKit` 提供的 API 进行开发，如果您对音视频数据的采集和处理有更多的需求，那么需要使用 `PLStreamingKit` 提供的 API 进行开发，不过在进行开发之前请确保您已经掌握了包括音视频采集，编码以及处理等相关的基础支持。


## 阅读对象

本文档为技术文档，需要阅读者：

- 具有基本的 iOS 开发能力
- 准备接入七牛云直播
