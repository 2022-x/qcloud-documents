## 概述

用户可将其静态资源（包括静态脚本、音视频、图片、附件等文件）全部托管在腾讯云 COS 的标准存储中，并利用无限容量、高频读写的特性，为静态资源提供可扩展和可靠的存储，减轻资源服务器的压力。COS 中的静态资源可接入 CDN 服务，由 CDN 进行全球加速，分发到用户客户端。

![](https://qcloudimg.tencent-cloud.cn/raw/2610b0a35199e10fcdcde9a4aded8356.jpg)

## 计费说明

COS 作为 CDN 源站时，含两部分计费：CDN 计费（加速）和 COS 计费（回源）。
![](https://qcloudimg.tencent-cloud.cn/raw/4eb89fb2ef76d6564b3e11413bbcb2e0.jpg)

### CDN 计费

当 CDN 进行加速服务，从 **CDN 节点**获取资源分发到**用户客户端**时（过程1和过程4），消耗的用量由 CDN 进行计费。详细计费说明请参见 [CDN 计费说明](https://cloud.tencent.com/document/product/228/2949)。

### COS 计费

当 CDN 回源，从 COS 源站获取资源（过程2和过程3），消耗的用量由 COS 进行计费。详细计费说明请参见 [COS 计费说明](https://cloud.tencent.com/document/product/436/16871)。

>! 非加速过程不涉及任何 CDN 流量费用。

