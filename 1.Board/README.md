[Wiki](https://wiki.sipeed.com/hardware/zh/maix/m1s/m1s_dock.html) ，[SDK](https://gitee.com/sipeed/M1s_BL808_SDK) (gitee)，[Examples](https://gitee.com/sipeed/M1s_BL808_example)（gitee），[Linux](https://github.com/sipeed/M1s_BL808_Linux_SDK)（Github）

---

#### 板卡特点

- 主芯片 BL808 RISC-V 480Mhz + NPU BLAI-100
- 板载 USB 转 UART 调试器（可实现一键点击烧录，无需按实体按键）
- 板载显示屏座子（可选配 1.69 寸 240x280 电容触摸屏）
- 板载 MIPI 摄像头座子（可选配 200W 像素摄像头）
- 支持 2.4G WIFI / BT / BLE
- 板载 1 个模拟麦克风、1 个 LED、1 个 TF 卡座
- 引出一路 USB-OTG 到 USB Type-C 接口

#### 硬件参数

<table>
    <thead>
        <tr>
            <th colspan="2"> M1s Dock </th>   
        </tr>
    </thead>
    <tbody>
    <tr>    
        <td rowspan="9" style="white-space:nowrap">主控 BL808 处理器</td>
    </tr>
    <tr>
        <td>多核 RISC-V (Max Freq 480MHz)</td>
    </tr>
    <tr>
        <td>AI NN 通用硬件加速器 —— BLAI-100 用于视频/音频检测/识别</td>
    </tr>
    <tr>
        <td>内嵌 64MB DRAM</td>
    </tr>
    <tr>
        <td>编解码：<br>- MJPEG and H264(Baseline/Main)<br>- 1920x1080@30fps + 640x480@30fps
        </td>
    </tr>
    <tr>
        <td>ISP（图像信号处理）：详情请查看芯片规格书</td>
    </tr>
    <tr>
        <td>接口：<br>- 摄像头接口 ：DVP 和 MIPI-CSI<br>- 显示接口：SPI、DBI、DPI(RGB)</td>
    </tr>
    <tr>
        <td>无线：<br>- 支持 Wi-Fi 802.11 b/g/n<br>- 支持 Bluetooth 5.x Dual-mode(BT+BLE)<br>- 支持 Wi-Fi / 蓝牙 共存</td>
    </tr>
    <tr>
      <td>USB 2.0 HS OTG （引出到 USB Type-C 接口）</td>
    </tr>
    <tr>    
        <td rowspan="5" style="white-space:nowrap"> 板载部件 </td>
    </tr>
    <tr>
        <td>板载 USB 转 UART 调试器（使用官方下载工具可实现一键点击烧录，无需按实体按键）</td>
    </tr>
    <tr>
        <td>板载 1 个显示屏座子（可选配 1.69 寸 240 x 280 电容触摸屏）</td>
    </tr>
    <tr>
        <td>板载 MIPI 摄像头座子（可选配 200W 像素摄像头）</td>
    </tr>
    <tr>
        <td>板载 1 个模拟麦克风、1 个 LED、1 个 TF 卡座 </td>
    </tr>
    <tr>    
        <td rowspan="5" style="white-space:nowrap"> 其他说明 </td>
    </tr>
    <tr>
        <td>外部供电需求 TYPE-C 接口：5V±10% 0.5A</td>
    </tr>
    <tr>
        <td>温升: &lt;30K</td>
    </tr>
    <tr>
        <td>工作温度范围:-10℃ ~ 65℃</td>
    </tr>
    </tbody>    
</table>

#### 产品对比

<table>
<thead>
<tr>
  <th style="text-align:left">项目</th>
  <th style="text-align:left">Maix Bit</th>
  <th style="text-align:left">ESP32 cam</th>
  <th style="text-align:left">M1s Dock</th>
</tr>
</thead>
<tbody>
<tr>
  <td style="text-align:left">处理器</td>
  <td style="text-align:left">K210</td>
  <td style="text-align:left">ESP32</td>
  <td style="text-align:left">M1s(BL808)</td>
</tr>
<tr>
  <td style="text-align:left">摄像头</td>
  <td style="text-align:left">0.3MP DVP GC0328</td>
  <td style="text-align:left">2MP DVP OV2640 with flash LED</td>
  <td style="text-align:left">2MP MIPI OV2685(two-side) with flash LED</td>
</tr>
<tr>
  <td style="text-align:left">显示屏</td>
  <td style="text-align:left">2.4 inch 320x240</td>
  <td style="text-align:left"></td>
  <td style="text-align:left">1.68 inch 280x240 带电容触摸</td>
</tr>
<tr>
  <td style="text-align:left">音频</td>
  <td style="text-align:left">I2S MEMS MIC</td>
  <td style="text-align:left"></td>
  <td style="text-align:left">Analog MEMS MIC + LineOut</td>
</tr>
<tr>
  <td style="text-align:left">SD 卡槽</td>
  <td style="text-align:left">SPI 模式</td>
  <td style="text-align:left">SPI 模式</td>
  <td style="text-align:left">· SDHC 模式 <br>· JTAG 模式</td>
</tr>
<tr>
  <td style="text-align:left">按键</td>
  <td style="text-align:left">Reset <br> Boot</td>
  <td style="text-align:left">Reset</td>
  <td style="text-align:left">· Reset <br>· Boot <br>· User x 2</td>
</tr>
<tr>
  <td style="text-align:left">USB</td>
  <td style="text-align:left">USB to Serial x 1</td>
  <td style="text-align:left"></td>
  <td style="text-align:left">· USB to Dual Serial x 1 <br>· USB OTG HS</td>
</tr>
<tr>
  <td style="text-align:left">其他</td>
  <td style="text-align:left"></td>
  <td style="text-align:left"></td>
  <td style="text-align:left">4P x 1.25mm 连接器（串口）</td>
</tr>
<tr>
  <td style="text-align:left">引脚</td>
  <td style="text-align:left">2 x 18 pins,可用于面包板</td>
  <td style="text-align:left">2 x 8 pins</td>
  <td style="text-align:left">2 x 16 pins,可用于面包板</td>
</tr>
<tr>
  <td style="text-align:left">JTAG</td>
  <td style="text-align:left"></td>
  <td style="text-align:left"></td>
  <td style="text-align:left">可选 TF2JTAG</td>
</tr>
<tr>
  <td style="text-align:left">外壳</td>
  <td style="text-align:left"></td>
  <td style="text-align:left"></td>
  <td style="text-align:left">可选</td>
</tr>
<tr>
  <td style="text-align:left">尺寸</td>
  <td style="text-align:left">25 x 53 mm</td>
  <td style="text-align:left">27 x 41 mm</td>
  <td style="text-align:left">27 x 55 mm</td>
</tr>
</tbody>
</table>

#### 软件描述

<table>
    <thead>
        <tr>
            <th colspan="2"> M1s Dock </th>   
        </tr>
    </thead>
    <tbody>
        <tr>
          <td>OS</td>
          <td>· 完备支持 FreeRTOS<br>· 基础支持 Linux</td>
        </tr>
        <tr>
          <td>开发方式</td>
          <td>· 原生 C SDK<br>· MaixHAL C 模块<br>· pikascript python 脚本</td>
        </tr>
        <tr>
          <td>固件下载</td>
          <td>· 串口下载<br>· 虚拟磁盘拖拽式更新</td>
        </tr>
        <tr>
          <td>AI 推理框架</td>
          <td>· 支持原生 SDK 的 BLAI 加速推理引擎<br>· 支持通用 TinyMaix 推理引擎</td>
        </tr>
        <tr>
          <td>AI 模型下载</td>
          <td>· <a herf="https://maixhub.com/">MaixHub</a> 下载。支持 人脸检测，识别，姿态检测，手势检测 等</td>
        </tr>
        <tr>
          <td>Sipeed 参考示例</td>
          <td>· https://gitee.com/sipeed/M1s_BL808_example</td>
        </tr>
    </tbody>
</table>

#### 算子支持列表

<table>
<thead>
<tr>
  <th>Type</th>
  <th>Operators</th>
  <th>Applicable Subset Spec.</th>
  <th>Processor</th>
</tr>
</thead>
<tbody>
<tr>
  <td rowspan="10">Convolution</td>
  <td rowspan="4">Conv </td>
  <td>Kernel: 1x1,3x3,5x5,7x7</td>
  <td rowspan="4">:strong:<code>NPU</code></td>
</tr>
<tr>
  <td>Stride: 1x1, 2x2</td>
</tr>
<tr>
  <td>Dilation: 1x1, 2x2</td>
</tr>
<tr>
  <td>Pad: same</td>
</tr>
<tr>
  <td rowspan="4">Depthwise Conv</td>
  <td>Kernel: 1x1,3x3 (5x5, 7x7 TBD)</td>
  <td rowspan="4">:strong:<code>NPU</code></td>
</tr>
<tr>
  <td>Stride: 1x1, 2x2</td>
</tr>
<tr>
  <td>Dilation: 1x1 (2x2 TBD)</td>
</tr>
<tr>
  <td>Pad: same</td>
</tr>
<tr>
  <td rowspan="2">Transpose Conv</td>
  <td>Kernel: 3x3</td>
  <td rowspan="2">strong:<code>NPU</code></td>
</tr>
<tr>
  <td>Stride: 2x2</td>
</tr>
<tr>
  <td rowspan="4">Pooling</td>
  <td rowspan="2">MaxPool (NPU TBD)</td>
  <td>Kerenl: 2x2</td>
  <td rowspan="2">DSP</td>
</tr>
<tr>
  <td>Stride: 2x2</td>
</tr>
<tr>
  <td rowspan="2">MaxPool</td>
  <td>Kerenl: 3x3</td>
  <td rowspan="2">:strong:<code>NPU</code></td>
</tr>
<tr>
  <td>Stride: 1x1, 2x2</td>
</tr>
<tr>
  <td rowspan="2">Activation</td>
  <td>Relu</td>
  <td></td>
  <td>:strong:<code>NPU</code></td>
</tr>
<tr>
  <td>Relu 6</td>
  <td></td>
  <td>:strong:<code>NPU</code></td>
</tr>
<tr>
  <td rowspan="5">Other processing</td>
  <td>BatchNormalization</td>
  <td>fused with conv</td>
  <td>:strong:<code>NPU</code></td>
</tr>
<tr>
  <td>Add (shortcut)</td>
  <td></td>
  <td>:strong:<code>NPU</code></td>
</tr>
<tr>
  <td>Concat (route)</td>
  <td>Channel wise (AXIS 3 in BHWC)</td>
  <td>:strong:<code>NPU</code></td>
</tr>
<tr>
  <td>Fully Connected</td>
  <td></td>
  <td>:strong:<code>NPU</code></td>
</tr>
<tr>
  <td>Upsample</td>
  <td>Nearest</td>
  <td>:strong:<code>NPU</code></td>
</tr>
</tbody>
</table>