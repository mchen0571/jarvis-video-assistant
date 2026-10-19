# 贾维斯视频助手 0.7.2

## 下载安装（按浏览器选择）

### Chrome：直接拖 ZIP，无需手动解压
**[点击下载 Chrome 拖拽安装包](https://github.com/mchen0571/jarvis-video-assistant/releases/download/v0.7.2/jarvis-video-assistant-0.7.2-chrome-drag.zip)**

1. 打开 `chrome://extensions`，开启右上角“开发者模式”。
2. 从电脑的文件管理器，将下载的 ZIP 拖进这个扩展管理页面；出现“拖放以安装”提示后松手。
3. 安装后打开含视频的网页，再点击扩展图标使用。

无需手动解压、无需修改系统策略。已在 Windows / Chrome 155 验证原生 ZIP 拖装、打开插件及退出重启后仍启用。包内保留候选阶段说明，当前验收结果以本页为准。运行文件与原版 0.7.2 逐文件一致；这里只验证安装方式，未重新验证所有网站下载功能。不要同时启用两份视频助手。

### Edge：目前仍需解压加载
**[点击下载 Edge 常规安装包](https://github.com/mchen0571/jarvis-video-assistant/releases/download/v0.7.2/jarvis-video-assistant-0.7.2.zip)**

解压到长期保留的文件夹，打开 `edge://extensions` 并开启开发人员模式，点击“加载解压缩的扩展”，选择其中的 `extension` 文件夹。

**本机 Edge 155 未通过直接拖 ZIP 安装，请勿把 Chrome 的通过结果当作 Edge 已支持。** 不提供被浏览器拒绝的自签 CRX，也不要求关闭安全检查或修改策略。

### 配套源码（不是安装包）
`jarvis-video-assistant-0.7.2-source.zip` 是开源许可配套源码和构建材料，普通使用无需下载。GitHub 自动生成的 `Source code (zip)` / `Source code (tar.gz)` 是仓库快照，也不是安装包。

运行于 Edge / Chrome 的 Manifest V3 视频下载扩展。无需本项目服务端，也无需另装本机后台程序。识别、下载和媒体处理在浏览器内进行；下载仍需访问视频所属网站。

## 功能边界
保留0.7.2交付版本的运行文件和处理流程。网站结构、访问权限和媒体编码变化可能导致识别或下载失败；不保证所有网站可用。知乎静态封面预览针对已验证播放器结构，不会自动播放或改变网页进度。请仅保存你有权下载和使用的内容。

## 隐私与权限
扩展包含 activeTab、scripting、storage、downloads、webRequest 权限，网站访问权限按需申请。运行中会在浏览器本地保存任务和媒体缓存，访问媒体网站时该网站仍会接收正常网络请求。无本项目服务端不等于不会访问互联网。

公开材料不包含开发者个人浏览记录、私人截图、账号凭据或内部测试数据。

## 许可与源码
原创代码采用 GPL-3.0-or-later。源码形式的 JavaScript、HTML、CSS 和清单随 extension 目录提供，无需编译即可加载。第三方源码与构建材料须与插件包一起提供明确的获取方式；具体版本与许可见 THIRD_PARTY_NOTICES.md。

插件包与配对源码包应在同一版本发布页免费提供。源码见 jarvis-video-assistant-0.7.2-source.zip。
