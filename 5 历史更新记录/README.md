## 历史记录

- 2.1.5 ([Release Notes](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/ReleaseNotes/release-notes-2.1.5.md) && [API Diffs](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/APIDiffs/api-diffs-2.1.5.md))
    - 缺陷
      - 修复推流预览在 app 退至后台一段时间后再返回前台时，有概率会卡住问题
      - 修复开启 VideoToolbox 编码时，退至后台再返回前台时，编码数据无法输出问题
      
- 2.1.4 ([Release Notes](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/ReleaseNotes/release-notes-2.1.4.md) && [API Diffs](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/APIDiffs/api-diffs-2.1.4.md))
  - 功能
    - 增加对 iOS 10 ReplayKit 录屏推流的支持
    - 增加 VideoToolbox 视频硬件编码功能
    - 增加人工报障和自动报障功能
  - 缺陷
    - 修复 iPhone 6s 及以上机型在 iOS 10 上的电流音问题
    - 修复 iPhone 6 及以上机型在 iOS 10 上同时开启自动对焦和手动对焦功能时，手动对焦失效问题
  - 优化
    - 优化 RGB 转 YUV 的效率，去除对 libyuv 库的依赖
- 2.1.3 ([Release Notes](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/ReleaseNotes/release-notes-2.1.3.md) && [API Diffs](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/APIDiffs/api-diffs-2.1.3.md))
  - 缺陷
    - 解决 iPhone 4s 及以下会 crash 的问题
- 2.1.2 ([Release Notes](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/ReleaseNotes/release-notes-2.1.2.md) && [API Diffs](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/APIDiffs/api-diffs-2.1.2.md))
  - 功能
    - 增加截屏功能
    - 增加自动网络检测功能
    - 增加自适应码率功能
    - 增加动态帧率功能
  - 缺陷
    - 修复音频未授权时 crash 的问题
    - 修复所有已知 crash
    - 修复前置摄像头无法缩放的问题
  - 优化
    - 优化不开美颜和水印时的性能
- 2.1.1 ([Release Notes](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/ReleaseNotes/release-notes-2.1.1.md) && [API Diffs](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/APIDiffs/api-diffs-2.1.1.md))
  - 缺陷
    - 修复与 PLPlayerKit v2.2.3 符号冲突的问题
- 2.1.0 ([Release Notes](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/ReleaseNotes/release-notes-2.1.0.md) && [API Diffs](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/APIDiffs/api-diffs-2.1.0.md))
  - 功能
    - 新增返听功能
    - 新增内置音效功能，支持十余种音效与数十个参数自由调节
    - 新增内置音频文件播放及混音推流功能
    - 新增外部视频图像处理本地预览功能
  - 缺陷
    - 修复分享到微博和 qq 空间时可能出现的卡 UI 的问题
    - 修复在流未连接的状态调用 restart 方法会出现只有视频没有声音的问题
    - 修复初始化时自动对焦不生效的问题
    - 修复一些偶发的 crash 问题
- 2.0.0 ([Release Notes](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/ReleaseNotes/release-notes-2.0.0.md) && [API Diffs](https://github.com/pili-engineering/PLMediaStreamingKit/blob/master/APIDiffs/api-diffs-2.0.0.md))
  - 功能
    - 提供 PLCameraStreamingKit 和 PLStreamingKit 两个层次的 API
    - 支持直接传入 stream URL 进行推流
    - 提供推流节点调度功能
    - 支持音频数据回调及处理功能
  - 缺陷
    - 修复orientation 在切换摄像头之后不起作用的问题
    - 修复初始化之后 inputGain 获取到的值始终为 0 的问题
    - 修复多种原因导致的死锁问题
    - 修复弱网推流可能出现的内存泄露问题
    - 修复特殊机器状态可能出现的 crash 问题
  - 优化
    - 优化对设备采样率的适配，推流过程中设备采样率变更将不再重新开始推流
- 1.8.1 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.8.1.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.8.1.md))
  - 功能
    - 更新依赖的 PLStreamingKit 到 1.2.5
    - 新增自动重连功能，默认关闭
    - 新增模拟器编译支持
    - 水印和美颜功能调整为支持 iPhone 5、iPad 3、iPod touch 4 及以上设备
  - 缺陷
    - 修复已知场景可能存在的没有声音的问题
    - 修复填充模式改变可能导致 preview 的 frame 发生改变的问题
    - 修复触摸屏幕对焦无效的问题
    - 修复无法正确设置采集相机位置的问题
    - 修复 capture session 设置不正确可能导致 crash 的问题
    - 修复偶尔出现的画面卡住无法正常推流的问题
- 1.8.0 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.8.0.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.8.0.md))
- 功能
  - 更新依赖的 PLStreamingKit 到 1.2.4
  - 新增内置美颜功能，美颜效果可调节
  - 新增单独调节前后置摄像头预览及推流是否镜像的接口
  - 新增动态帧率功能，通过降低采集帧率来适配弱网环境
- 缺陷
  - 修复音视频时间戳偶尔出现的非单调递增的缺陷
  - 修复特殊机型可能出现的没有声音的问题
- 优化
  - 优化水印性能，降低 CPU 和内存消耗
- 1.7.2 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.7.2.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.7.2.md))
  - 功能
    - 更新依赖的 PLStreamingKit 到 1.2.2
    - 新增回调队列配置功能
    - 新增默认摄像头位置配置项
    - 新增录制音量调节选项（由于系统原因，仅对除 iPhone 6s 系列以外的机型生效）
    - 支持初始化的时候传入 stream 为 nil
    - 支持快速重连操作，方便 4G 推流时切换 WIFI 场景快速切换网络
  - 缺陷
    - 修复特殊场景可能出现的电流音问题
    - 修复特殊场景可能出现的没有声音的问题
    - 修复后台推流时被音频打断结束之后无法正常恢复推流的问题
- 1.7.1 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.7.1.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.7.1.md))
  - 缺陷
    - 修复切换前置摄像头之后无法缩放的问题
    - 修复不添加水印无法正常推流的问题
- 1.7.0 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.7.0.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.7.0.md))
  - 功能
    - 新增后台推流功能（仅音频，因 iOS 隐私限制不允许后台访问摄像头）
    - 新增水印功能
    - 新增可选定制美颜功能（需联系工作人员）
  - 缺陷
    - 修复特定机型上的电流音等杂音问题
  - 版本
    - 更新依赖 PLStreamingKit 的版本到 `v1.2.0`
  - 其他
    - 部分接口重命名
- 1.6.3 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.6.2.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.6.2.md))
    - 更新依赖 PLStreamingKit 的版本到 `v1.1.6`
    - 更新 Demo 适应 PLStreamingKit `v1.1.6` 接口变更
- 1.6.2 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.6.2.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.6.2.md))
    - 更新依赖 PLStreamingKit 的版本到 `v1.1.5`
    - 支持 Zoom 操作
- 1.6.1 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.6.1.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.6.1.md))
    - 更新依赖 PLStreamingKit 的版本到 `v1.1.3`
    - 修复调用 `- (void)reloadVideoConfiguraiton` 方法，fps 变更失败的问题
- 1.6.0 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.6.0.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.6.0.md))
    - 更新依赖 PLStreamingKit 的版本到 `v1.1.2`
    - 添加 `PLStreamStatus` 回调，便于客户端监控推流状态
    - 修复采集源 fps 变更失败的问题
- 1.5.2 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.5.2.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.5.2.md))
    - 更新依赖 PLStreamingKit 的版本到 `v1.0.3`
- 1.5.1 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.5.1.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.5.1.md))
    - 更新依赖 PLStreamingKit 的版本到 `v1.0.2`
    - 更改音频数据源采集部分，转换为单声道
- 1.5.0 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.5.0.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.5.0.md))
    - 编码推流改为依赖 `PLStreamingKit`
    - 去除 `PLAudioStreamingSession` 类, 建议单纯推音频的 App 直接接入 `PLStreamingKit`
    - 摄像头及音频采集部分开源
    - 底层添加了 HappyDNS, 解决部分地区 DNS 感染严重导致推流失败问题
    - 优化 TCP 层发包，极大程度解决了网络正常但推流中经常断开的问题
- 1.4.16 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.16.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.16.md))
    - 解决 destroy 方法可能卡死线程的问题
- 1.4.15 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.15.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.15.md))
    - 修复类库 .a 未更新问题
- 1.4.14 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.14.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.14.md))
    - 解决视频质量切换时导致 crash 的问题
    - 解决推流时触发的只有音频无视频问题
    - 解决音频采样导致的电流声
    - 解决潜在内存问题，整体提升稳定性
    - 视频编码统一 profileLevel 为 baseline31
    - 限定最高支持分辨率到 720p
- 1.4.13 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.13.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.13.md))
    - 更新 mute 行为，mute 后不会中断发包
    - 更新音频设备采样率获取途径
    - 更新底层库，避免冲突
- 1.4.12 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.12.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.12.md))
    - 添加 `smoothAutoFocusEnabled` 参数，确保拍摄时对焦的平滑过渡
    - 修复无网络环境或其他情况触发断流时引起的 crash
    - 修复频繁切换摄像头时引起的 crash
    - 修复内存 leak
- 1.4.11 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.11.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.11.md))
    - 修复 iPhone 6s 系列机型直播无声音问题
- 1.4.10 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.10.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.10.md))
    - 修复错误重连或者主动重连时导致 UI 卡顿的问题
- 1.4.9 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.9.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.9.md))
    - 尝试修复 iPhone 6s 音频获取不到权限的问题
    - 优化丢包策略，兼顾高延时和低带宽的情况
    - 更新 demo 为全异步请求
- 1.4.8 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.8.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.8.md))
    - 尝试修复 iPhone 6s 音频获取不到权限的问题
    - 修复弱网环境触发的内存和 CPU 占用升高的问题
- 1.4.7 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.7.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.7.md))
    - 尝试修复音频获取不到权限的问题
    - 添加关闭 SDK 渲染 preview 的接口
- 1.4.6 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.6.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.6.md))
    - 修复弱网环境下切换 VideoQuality 可能触发的 crash 问题
    - 添加 `PLAudioComponentFailedToCreateNotification` 通知，在音频资源被占用时，创建音频结构失败会发送这个通知
- 1.4.5 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.5.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.5.md))
    - 添加自行绘制 CMSampleBufferRef 的支持
- 1.4.4 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.4.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.4.md))
    - 为 PLCameraStreamingSession 多个属性添加 kvo 支持
    - 由时间计数改为包数计数
    - 针对弱网坏境更改丢帧策略，确保不会出现花屏和声音抖动，取而代之会出现间断的无数据，但是可以保证画面和声音的流畅
    - 发送队列的默认上下阈值更改为 0.3 和 0.7
- 1.4.3 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.3.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.3.md))
    - 优化网络层调用，添加 `Disconnecting` 流状态
    - 抽离可导致推流中断的错误
    - 添加错误回调，同时将错误信息返回，便于 debug 及异常处理
    - 修复 `destroy` 调用导致的崩溃问题
    - 支持 iOS 9 的 bitcode
- 1.4.2 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.2.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.2.md))
    - 添加 SendingBuffer 支持
    - 修复 iPhone 6s 下崩溃的问题
- 1.4.1 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.1.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.1.md))
    - 添加可以获取视频源数据的回调方法，便于开发者做滤镜等处理
    - 对自定义分辨率做了内部修正，保证宽高均为 16 倍数
- 1.4.0 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.4.0.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.4.0.md))
    - 添加音频推流的 `PLAudioStreamingSession`, 纯音频推流合并到 `PLCameraStreamingKit`
    - 添加后台推流支持，暂且只在纯音频推流中有效
- 1.3.2 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.3.2.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.3.2.md))
    - 修复直播被电话 / 闹钟中断后后续直播无声音的问题
    - 更改音频采集类型: RecordAndPlay -> Record
    - 添加对蓝牙音频设备的支持
- 1.3.1 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.3.1.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.3.1.md))
    - 修复调用 destroy 方法后，重新创建 session 进入后台触发的 crash 问题
    - 去除无用依赖, SDK 大小由 17 MB 降低为 4.7 MB
- 1.3.0 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.3.0.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.3.0.md))
    - 添加带宽质量检测机制，推流过程中可无缝切换音视频 Quality，实现码率及帧率的动态调节
    - 添加发送队列的配置及状态回调
    - 更新 Example 来简单说明如何使用发送队列和 Quality 组合推流策略
- 1.2.8 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.2.8.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.2.8.md))
    - 更新编码配置，分离音视频编码配置，便于提供更灵活的配置方案
    - 去除 SIGPIPE 断点
    - 修复 URL 错误时导致的崩溃
    - 修复创建 Session 后设置 Stream 推流失败的问题
- 1.2.7 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.2.7.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.2.7.md))
    - 修复断网后停止流时导致的 UI 卡死
    - 修复停止推流时概率出现的 crash 问题
    - 添加 `- (void)destroy` 方法到 `PLCameraStreamingSession`
    - 暂且去除 iOS 8 编码，待进一步优化后再做开放
    - 修复反复进出持有 streamingSession 的 viewController 出现 IO 错误或者 crash 的问题
- 1.2.6 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.2.6.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.2.6.md))
    - 修复 iOS 8 以下推流时，编码导致的崩溃问题
- 1.2.5 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.2.5.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.2.5.md))
    - 更新了 Quality 配置
- 1.2.4 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.2.4.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.2.4.md))
    - 添加全新的 iOS 8 硬编码器，减少编码延时
- 1.2.3 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.2.3.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.2.3.md))
    - 更新了 `PLStream` 类结构
    - 添加新的 session 创建接口
    - 移除 publishHost，`PLStream` 对象支持自动生成推流地址，请搭配服务端 SDK 至少 1.2.0 或以上版本使用
- 1.2.2 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.2.2.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.2.2.md))
    - 更新麦克风资源调用方式，添加进入后台后自动停用麦克风功能
- 1.2.1 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.2.1.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.2.1.md))
    - 修复初次授权摄像头后预览界面为黑屏的问题
- 1.2.0 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.2.0.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.2.0.md))
    - 添加了 `PLStream` 类，支持 `Coding` 协议便于打包存储
    - 更新 `StreamingSession` 创建方法，借助传递 `PLStream` 对象再无需推流时等待服务端生成推流地址
    - 完善 HeaderDoc 文档
- 1.1.8 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.1.8.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.1.8.md))
    - 添加摄像头开启和关闭的操作，便于开发者控制 AVCaptureSession
- 1.1.7 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.1.7.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.1.7.md))
    - 添加推流质量字段，方便开发者指定推流质量
    - 移除原配置中的网络选项
    - 默认情况下关闭了 PLLog
    - 添加摄像头开始运行的通知
    - 添加麦克风开始运行的通知
- 1.1.6 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.1.6.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.1.6.md))
    - 尝试修复音频变声问题
- 1.1.5 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.1.5.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.1.5.md))
    - 修复了重连后无法播放的问题
- 1.1.4 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.1.4.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.1.4.md))
    - 更新了码率和采样率。现在统一使用 128Kbps 和 44100KHZ，用以解决噪音的问题
    - 更新了网络 socket。对 socket 在调试情况下出现的 SIGPIPE 进行了处理，不会再出现
    - 更新了网络状态的返回情况。当不是主动调用 close 接口导致的断开都将以 error 状态通知 delegate
- 1.1.3 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.1.3.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.1.3.md))
    - 更新了获取视频截图的方法
    - 添加 HeaderDoc 格式注释文档
- 1.1.2 ([Release Notes](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/ReleaseNotes/release-notes-1.1.2.md) && [API Diffs](https://github.com/pili-engineering/PLCameraStreamingKit/blob/master/APIDiffs/api-diffs-1.1.2.md))
    - 添加自定视频大小的编码配置
    - 添加进入后台后自动停止推流的支持
    - 添加保持常亮的开关
    - 添加获取当前录制截屏的功能
    - 修复进入后台导致崩溃的问题
    - 修复切换前置摄像头失效的问题
    - 添加 Release Notes 说明每个版本变动
    - 添加 API Diffs 说明具体修改细节
- 1.1.1
    - 修复 release 版本无法推流的 bug
    - 内存优化，比 1.1.0 减少 6% 左右内存消耗
- 1.1.0
    - 重构接口
    - 优化编码参数
    - 提供不同网络和分辨率下的多种配置可选
    - 添加消息通知，便于监听
    - 兼顾 arc 及非 arc 的工程
- 1.0.0
    - 发布 CocoaPods 版本