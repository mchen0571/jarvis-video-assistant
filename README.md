# 贾维斯视频助手 0.7.2

在 Edge / Chrome 中识别和下载网页视频，自动选择最高画质、保留原音。媒体处理在浏览器内完成，无需另装后台程序。

## 下载

**[下载插件安装包（Edge / Chrome 通用）](https://github.com/mchen0571/jarvis-video-assistant/releases/download/v0.7.2/jarvis-video-assistant-0.7.2-drag-install.zip)**

普通使用只需下载这一个 ZIP，**不用手动解压，也不用下载源码包**。

## 安装

### Microsoft Edge
1. 在地址栏打开 `edge://extensions`，开启“开发人员模式”。
2. 从电脑的文件管理器，把下载的 ZIP 拖到页面上部 **“已安装的扩展”标题附近的内容区域**。
3. 看到 **“拖放以安装”** 后松开鼠标，等待扩展出现并保持开启。

**不要拖到页面底部的大块空白处。** 如果没有出现安装提示，按 Esc 取消，再移到上部内容区域操作。

### Google Chrome
1. 在地址栏打开 `chrome://extensions`，开启“开发者模式”。
2. 从文件管理器把 ZIP 拖进扩展管理页面，看到 **“拖放以安装”** 后松开鼠标。

安装后请保持开发者模式开启。若浏览器询问是否关闭该模式，选择保留。

## 使用

打开目标视频网页，必要时先播放视频，再点击浏览器工具栏中的“贾维斯视频助手”。按提示授予所需网站访问权限，找到对应视频后点击下载。

可在浏览器的扩展菜单中将它固定到工具栏。请勿同时启用多份视频助手。

## 使用范围

- 已在 Windows 的 Edge 155 和 Chrome 155 验证 ZIP 拖拽安装、打开扩展以及重启后保持启用。
- 网站结构、访问权限和媒体编码变化可能影响识别或下载，不保证所有网站可用。
- 请仅下载你有权保存和使用的内容。
- GitHub 分发不提供扩展商店式自动更新。

<details>
<summary>备用安装方式与其他附件</summary>

如果无法拖拽安装，可将通用安装包完整解压到长期保留的文件夹，在扩展管理页点击“加载解压缩的扩展”，选择直接包含 `manifest.json` 的根文件夹。安装后不要移动或删除该目录。

发布页下方其他文件的用途：
- `jarvis-video-assistant-0.7.2-source.zip`：配套源码与构建材料，不是安装包。
- `SHA256SUMS.txt`：文件完整性校验值，普通使用可不下载。
- `jarvis-video-assistant-0.7.2-chrome-drag.zip`：旧命名安装包，与通用拖装包内容相同，为兼容旧下载链接保留。
- `jarvis-video-assistant-0.7.2.zip`：旧版打包结构，解压安装时选择其中的 `extension` 子文件夹。
- GitHub 自动生成的 `Source code (zip)` / `Source code (tar.gz)`：仓库快照，不是插件安装包。

</details>

<details>
<summary>已知问题</summary>

扩展管理页可能记录一条关于 `webRequest` 缺少网站权限的警告。该警告未阻止已验证的安装、启用和弹窗打开；网站下载行为仍受实际授权及网站兼容性影响。当前版本保留该问题，未额外扩大网站权限。

安装包内部分说明仍保留早期候选阶段文字，最新安装方法以本页为准。

</details>

## 隐私与权限

扩展使用 `activeTab`、`scripting`、`storage`、`downloads`、`webRequest` 权限，网站访问权限按需申请。任务与媒体缓存保存在浏览器本地；下载时仍需访问媒体所属网站，该网站会接收正常网络请求。扩展不需要本项目服务端。

## 开源许可与源码

原创代码采用 **GPL-3.0-or-later**，第三方组件保留各自许可，详见 `THIRD_PARTY_NOTICES.md`。JavaScript、HTML、CSS 和清单随通用安装包根目录提供。

**[获取配套源码与构建材料](https://github.com/mchen0571/jarvis-video-assistant/releases/download/v0.7.2/jarvis-video-assistant-0.7.2-source.zip)**。普通使用无需下载；如需研究、修改或再分发，请同时阅读相关许可及源码材料。
