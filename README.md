# Kianu De-noise

面向人声/对白的实时降噪插件（VST3 + 独立程序），Windows x64。

![界面预览](docs/screenshot.png)

---

## 功能

- **实时谱减降噪**：低延迟，适合直播、录音、后期对白清理
- **噪声学习**：点一下 `LEARN NOISE` 抓取当前底噪轮廓，随工程保存
- **三档工作模式**：Dialogue（对白）/ Balance（均衡）/ Music（音乐）
- **可视化对比**：波形区同时显示 INPUT（灰）与 OUTPUT（青绿），一眼看出被削掉的部分
- **阈值直接在波形上拖**：虚线即阈值，上下拖动即可改，双击复位
- **旋钮拖动时显示数值**：不占版面，松手即收起

| 参数 | 范围 | 说明 |
|---|---|---|
| Threshold | −60 … 0 dB | 低于此电平的噪声被处理 |
| Reduction | 0 … 100 % | 降噪强度 |
| Range | 0 … 60 dB | 最大衰减量 |

## 安装

1. 到 [Releases](../../releases) 下载最新的 `Kianu De-noise v1.0.0 (Windows x64).zip`
2. 安装后会把 `Kianu De-noise.vst3` 放到：

   ```
   C:\Program Files\Common Files\VST3\
   ```

3. 在宿主（Cubase / Studio One / Reaper / FL Studio / Audition…）里重新扫描插件
4. 也可以直接运行 `Kianu De-noise.exe` 用独立程序

## 使用

1. 先播一段「只有噪声、没有人声」的素材，点 `LEARN NOISE`（3 秒自动结束）
2. 播放正式素材，看波形上的灰色 INPUT 是否被压在虚线以下
3. 拖虚线上/下调整阈值，或转 `REDUCTION` / `RANGE`
4. 三种模式按素材切换：人声用 Dialogue，混合内容用 Balance，音乐用 Music

![拖动旋钮读数](docs/knob-drag.png)

## 系统要求

- Windows 10 / 11 x64
- 支持 VST3 的宿主，或直接使用独立程序

## 反馈

有问题、想要新功能，加微信：**fenderstudiopro**

<img src="Data/wx.jpg" width="180" alt="微信二维码">

## 声明

内核源自网络，仅供学习研究使用。请勿商用或用于非法用途，后果自负。喜欢请支持正版，侵权请微信联系我们处理。
完整条款见 [LICENSE](LICENSE)。

## 从源码构建

```bash
自己动手，丰衣足食
```

KIANU AUDIO · 2026
