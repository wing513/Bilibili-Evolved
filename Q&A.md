# 常见问题

## 左侧没有设置等按钮 / 页面没有任何变化

- 检查脚本是否安装完整, 可以在[首页](https://github.com/the1812/Bilibili-Evolved#安装)中使用不同的安装源重新安装.
- 检查浏览器是否支持, 此脚本仅支持高版本的原版Chrome, Edge (Chromium 内核), Firefox, Safari.

## 下载视频相关

### 直接下载时标签页崩溃 / 报错 "File could not be read"

直接下载过程中所有数据都存在内存里, 不同浏览器可以存放1~2G左右, 太大的视频就会导致标签页崩溃或报错. 可以考虑使用`显示链接`转给IDM或浏览器下载, 或使用[导出 aria2](aria2-notice.md)来进行下载.

### 下载时报错: 获取下载链接失败

有多种可能原因:
- 账号权限不足:
  - 1080P 720P 需要登录账号
  - 1080P60 1080P+ 720P60 需要大会员账号
- 片源没有对应格式: 例如老视频仅有`FLV`格式, 选择`DASH`格式就会失败, 请更换格式.

### 港澳台番剧没有下载按钮

如果以您的账号权限无法观看某些视频(地区限制, 大会员专享等), 就算使用了类似[解除B站区域限制](https://greasyfork.org/zh-CN/scripts/25718-%E8%A7%A3%E9%99%A4b%E7%AB%99%E5%8C%BA%E5%9F%9F%E9%99%90%E5%88%B6)的脚本也是无法下载的, 除非您有对应节点的梯子.

### 番剧没有弹幕

部分用户在同时开启此脚本和[解除B站区域限制](https://greasyfork.org/zh-CN/scripts/25718-%E8%A7%A3%E9%99%A4b%E7%AB%99%E5%8C%BA%E5%9F%9F%E9%99%90%E5%88%B6)脚本后, 会出现番剧没有弹幕的问题, 目前没有解决方法.

### 如何得到 MP4 格式

下载时选择`DASH`格式(注意只有新一点的视频才支持, 老视频只有`FLV`), 得到视频和音频文件后用 [ffmpeg](https://ffmpeg.org/) 合并, 合并方法见[#183](https://github.com/the1812/Bilibili-Evolved/issues/183).
