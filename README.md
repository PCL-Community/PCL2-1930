<!--
 ____     ____       __           ___       __ __         _        __         __        __     
/\  _`\  /\  _`\    /\ \        /'___`\    _\ \\ \__    /' \     /'_ `\     /'__`\    /'__`\   
\ \ \L\ \\ \ \/\_\  \ \ \      /\_\ /\ \  /\__  _  _\  /\_, \   /\ \L\ \   /\_\L\ \  /\ \/\ \  
 \ \ ,__/ \ \ \/_/_  \ \ \  __ \/_/// /__ \/_L\ \\ \L_ \/_/\ \  \ \___, \  \/_/_\_<_ \ \ \ \ \ 
  \ \ \/   \ \ \L\ \  \ \ \L\ \   // /_\ \  /\_   _  _\   \ \ \  \/__,/\ \   /\ \L\ \ \ \ \_\ \
   \ \_\    \ \____/   \ \____/  /\______/  \/_/\_\\_\/    \ \_\      \ \_\  \ \____/  \ \____/
    \/_/     \/___/     \/___/   \/_____/      \/_//_/      \/_/       \/_/   \/___/    \/___/ 
                                                                                               
欢迎来到这个文档，正如您所见，这是 PCL2 仓库 Discussion #1930 的源码。
因为只能使用 Markdown，所以这个文档的排版非常难受，我已经尽可能使其看得可以顺眼一些了qwq……
我只公布了表格正文部分，其他部分就先不公布了，意义不是很大。（看起来还是有必要的…… 有一回手残把前面的删掉了时隔快一个月才发现，又重写了一遍…… 那就把整理起来比较坐牢的地方公布一下，也当作针对我自己的防呆措施 Owo）
如果您希望可以直接参与到这里来补充这个表格，可以直接往这个仓库丢 PR，我会在周末进行同步更新的。
嗯…… 显然，您是没法在这里交有关这个表格的 Issue 的，直接去原页面下方丢评论就好啦。
-->

## PCL2 常见&难检反馈及问题列表

### 注意事项

- 请仔细阅读 [关于](ABOUT.md)！当您阅读或者贡献本仓库以及原始 Discussion 的内容后即默认您已阅读并同意该文件提及的全部内容。
- 对于组织内成员，请不要直接修改此文件！**请在 Fork 后提交 Pull Request** 来完善本文档，而不是在此仓库创建新 Branch，这可能会触发分支保护规则而复杂化您的操作流程。

### 特别鸣谢

![Contributors](https://contrib.rocks/image?repo=PCL-Community/PCL2-1930)

##### [◆ 辅助管理权限说明](https://github.com/Hex-Dragon/PCL2/discussions/477) [◆ 讨论时的常见疑惑](https://github.com/Hex-Dragon/PCL2/discussions/775) [◆ 声明：请不要为了获取权限而活跃](https://github.com/Hex-Dragon/PCL2/discussions/3666) [◆ 简介：PCL 功能投票](https://github.com/Hex-Dragon/PCL2/discussions/2) [◆ 内部管理沟通帖](https://github.com/Hex-Dragon/PCL2/discussions/1952) [◆ PCL2 帮助库](https://github.com/LTCatt/PCL2Help) [◆ Hex-Dragon Discord 服务器](https://discord.gg/npstwgmftR) [◇ 主页标准与指导](https://github.com/Hex-Dragon/PCL2/discussions/4483) [◇ PCL 各平行版本指南](https://github.com/Hex-Dragon/PCL2/discussions/3933) [◇ 遥遥无期的联机的相关情报公开](https://github.com/Hex-Dragon/PCL2/discussions/4166) [◇ 致各位：一些交流方面的建议 ◇](https://github.com/Hex-Dragon/PCL2/discussions/1592)

<!-- 表格正文于此开始。-->

### Minecraft 常见问题

 <!-- BUILD_FLAG:BEGIN Minecraft -->
 | 内容 | 解释 | 参考 |
 |--|--|--|
 | **无法下载 Minecraft** | **为 MCBBS 关停所致，同时由于 BMCLAPI 源压力过大，可能导致大部分时间段无法通过镜像源下载 Minecraft。届时请尝试以下四种解决方案：<br>1. 更换不同的网络；<br>2. 每间隔一段时间后再次尝试下载；<br>3. 若您的网络条件允许，尝试使用加速器或 VPN；<br>4. 如个人技术能力允许，尝试部署 [OpenBMCLAPI](https://github.com/bangbang93/openbmclapi)。** <br><br>*部分日志可见：`基础连接已经关闭: 未能为 SSL/TLS 安全通道建立信任关系。`* | **[Bilibili&nbsp;动态](https://t.bilibili.com/899749241434406921)** <br> #3213
 | **1.16.4 及 1.16.5 离线模式无法进入多人游戏界面** | **PCL 不会解决该问题，这超出了启动器功能范畴。** <br> *如仍需要使用多人游戏 [^1]，请自行断网启动游戏或安装 [MultiOfflineFix](https://github.com/MCTeamPotato/MultiOfflineFix "Fabric & Forge") 或 [Offline Multiplayer](https://github.com/ChickenPige0n/offline-multiplayer-fabric "仅 Fabric") Mod。同时您可以参考 [此处的解决方案](https://github.com/Hex-Dragon/PCL2/discussions/1930#discussioncomment-6797858) 以彻底解决此问题。* | **PCL2&nbsp;内置帮助库 <br> #2003 #2017 #2004 [#1930](https://github.com/Hex-Dragon/PCL2/discussions/1930#discussioncomment-6805733)**
 | 游戏崩溃 | 请依照本文下方附文步骤进行解决。
 | 无法进入服务器 | 非 PCL 问题，具体可能的解决方案见内置帮助库或前往相关论坛寻求他人帮助。 | PCL2&nbsp;内置帮助库
 | 部分时段无法登录正版账户但网络速度良好 | 可能为使用中国联通或中国移动网络下 `api.minecraftservices.com` 和二级域名为 `mojang.com` 的地址均被屏蔽所致，请尝试使用中国电信网络或使用 VPN。 | #2738
 | 游戏内无法正确加载皮肤 | 请检查您的网络环境，使用加速器或 VPN。 | -
 | 整合包中安装了 OptiFine 导致游戏无法正常加载 | OptiFine 和 Mod 加载器之间存在严重的兼容性问题，请考虑只安装 OptiFine 或只安装 Mod 加载器，亦或是使用其他 Mod 替代 OptiFine。 | #3258 #3566 #3573 MCLF-CN/docs#6
 | 游戏无声音 | 在未静音的情况下，请尝试 “版本设置 → 高级管理 → 补全文件”，若问题仍未解决，则尝试关闭 Windows 防火墙后再试。 | #4368
 | 1.12 及以下 OptiFine Forge 版本窗口大小和设置值不同 | 此为第三方组件在启动过程中使用了不同的算法处理传入的窗口大小所致。PCL 对该问题进行的修复仅对原版生效，将不再受理 **1.12.2-**、**OptiFine/Forge** 下窗口大小和设置的尺寸不同的 Bug。| #3463
 <!-- BUILD_FLAG:END Minecraft -->


### 启动器常见问题

 <!-- BUILD_FLAG:BEGIN PCL -->
 | 内容 | 解释 | 参考 |
 |--|--|--|
 | **支持通过启动器联机游玩 Minecraft** | ***“至于联机，因为网易还在继续代理中国版，我和 HMCL 的维护者都觉得还得谨慎一点……况且现在也有 Mod 支持联机了……咳咳。”*** <br> ***“目前联机并不是遇到了技术问题。等到网易不代理国服了联机就有了”*** <br> <div align="right"> ***——龙腾猫跃*** </div> <br> *BakaXL 现已于 2023 年 10 月 8 日将其部分服务与 Octo 章鱼网络进行对接，并对其可用性进行初步评估，待评估完成后，Octo 网络会全面对其他启动器开放。*[^4]  | **[2.6.11&nbsp;更新日志](https://www.bilibili.com/read/cv28121157/)** #4166 [#4158](https://github.com/Hex-Dragon/PCL2/discussions/4158#discussioncomment-9968069)
 | **支持启动器多语言选项**<br>**· I18n support & Support more languages** | **社区正在进行翻译工作，已有相关 Pull Request。**<br>**· The community is working on translation. Related pull request already exists.**<br>*如若您需要多语言版本，请见 #4580。*<br>*· You can download the multi-language version at #4580.* | 🔹 **#4145** <br> #891 #4580
 | PCL 消失、报毒、无法更新 | 为 Microsoft Defender 和 360 等杀毒软件误报，请在 Windows 安全中心和杀毒软件中添加排除项或白名单。具体教程见 PCL 内置帮助库。 |  PCL2&nbsp;内置帮助库 <br> #56 [#666](https://github.com/Hex-Dragon/PCL2/issues/666#issuecomment-1611534587)
 | 以管理员权限运行时无法使用文件拖拽功能 | **[需要社区帮助]** *“尽可能尝试修复相关代码，依然无法解决……如果谁有解决方案可以提出”* ——龙腾猫跃 | [#2531](https://github.com/Hex-Dragon/PCL2/issues/2531#issuecomment-1822511620)
 | 增加导出整合包功能 | 已有相关 Pull Request。 | 🔹 **#4758** <br> #98
 | 支持启动基岩版（BE）、教育版、传奇（Minecraft Legends；MCL）、地下城（Minecraft Dungeons；MCD）等其他 Minecraft 衍生游戏 | *“这玩意儿我根本启动不了！用官方启动器吧！告辞！” ——龙腾猫跃* | #81
 | 支持第三方登录全局设置 | 正在 Discussions 中投票。 | #57 (#58)
 | 支持更新整合包 | 正在 Discussions 中投票。 | #5068 (#5069)
 | 爱发电无法收到加群信息或更新密钥 | 加群请 **在爱发电** 回复 “加群”，更新密钥 **在爱发电** 获取请回复 “‘更新’ +识别码”。如无法收到回复，很可能是您已经触发了人工回复，在等待人工回复的过程中无法使用命令。您如果只是想使用命令，可以发送 “取消人工处理”。如仍旧没有回复，可以等待一会后再进行尝试。 | [石墨文档](https://shimo.im/docs/qKPttVvXKqPD8YDC) <br> #1867 #1529
 | 使用自定义主页时出现问题 | 一般情况下非启动器问题，为第三方主页问题，请联系主页作者。<br>*对于启动器内置的预设主页，请见下方 “预设主页” 部分获取对应作者及其仓库。* | #3393 #3002 #2930 等 Issues
 | 支持 macOS、Linux、iOS、Android 等其他操作系统 | PCL 的底层界面框架（WPF）无法跨系统，要兼容其他系统无异于完全重做，不会制作。 | #54
 | 添加皮肤库 | 不会制作该功能。 | #343
 | 支持离线披风 | 技术上无法实现。 | #700
 | 支持调整 OptiFine 和第三方披风选项 | 暂时不打算制作。 | #2045 #2065
 | 支持离线模式下 1.19.3+ 版本自定义皮肤 | 正在 Discussions 中投票。 | #1288 (#1596)
 | Minecraft 更新后 PCL 内未找到该最新版本 | 请在 **“设置 → 启动器 → 下载 → 版本列表获取”** 选择 **“尽量使用官方源”**。 | #1226
 | 支持识别、安装 Quilt | 已有相关 Pull Request。 | 🔹 **#4074** <br> #48
 | 支持识别、安装 Cleanroom | 正在 Discussions 中投票。 | #3003 (#3004)
 | 支持识别、安装 OptiKai | 正在 Discussions 中投票。 | #3881 (#3882)
 | 支持安装 Legacy Fabric、Legacy Fabric API、Babric 等 | 已不再考虑专门为 Minecraft 1.9 及以前的版本追加新功能。 | #3171 #283
 | 支持修改已安装版本的组件和 Mod 加载器 | 正在 Discussions 中投票。<br> *搜索关键词：Fabric、Forge、OptiFine、LiteLoader、NeoForge、Quilt。* | #220 (#227)
 | 安装整合包时支持修改 Mod 加载器版本 | 修改 Mod 加载器版本可能会导致严重的兼容性问题，请联系整合包作者解决，PCL 不会支持该功能。 | #3568
 | 支持下载资源包（纹理包/材质包） | 已有相关 Pull Request。 | 🔹 **#4020** <br> #44
 | 支持下载光影包 | 已有相关 Pull Request。 | 🔹 **#4359** <br> #396
 | 支持下载数据包 | 正在 Discussions 中投票，已有相关 Pull Request。 | 🔹 **#4360** <br> #2991 (#2994)
 | 支持下载地图 | 存在语言问题，不会制作。 | #44 #135
 | 支持下载第三方服务端及插件 | PCL 是启动器，此功能超出了启动器的范畴。 | #108
 | 支持下载特定版本的 Java | 没有合适的下载源，暂不考虑。 | #3585
 | 引进新 Mod / 整合包下载源 | 没有其他可用的国内的 API。 | #1658
 | 允许管理存档、截图、资源包、光影包等文件 | 已有相关 Pull Request。 | 🔹 **#4770**
 | 支持导出 Mod 列表 | 该功能可以被导出整合包基本覆盖，暂不考虑制作。 | #2586
 | 添加 Mod 收藏夹 | 正在 Discussions 中投票，已有相关 Pull Request。 | 🔹 **#4933** <br> #487 (#1646)
 | Mod 管理支持分类 Mod | 不会制作。<br>*搜索关键词：分类、分组、模组、管理、分区、收藏、文件夹、收藏夹、星标。* | #277
 | 无法搜索到指定 Mod & Mod 搜索筛选选项异常 & Mod 搜索匹配版本错误 & Mod 详情页前置问题 等 Mod 搜索问题 | 为 API 或 Mod 作者上传时的设置问题，PCL 无法解决。[^2] | #2352 #2277 #2190 #2069 等 Issues
 | 无法加载部分来自 Modrinth 的 Mod 图标 | 此类 Mod 使用了 SVG 格式的图标，PCL 不考虑支持此类图标。 | #1409
 | PCL 无法访问 Modrinth，但浏览器能正常访问 | 目前已无法复现，如有遇到此类现象可在 #4334 评论。 | #4334
 | 下载或安装资源时失败 | 请先尝试使用其他启动器下载，若使用后问题依然存在，则非 PCL 问题。请使用镜像源或检查您的网络环境，使用加速器或 VPN。<br>如若确定网络环境无问题，请尝试设置游戏 Java 为最新版本的 Java 后再试。 | #3211
 | 支持下载或安装资源时断点续传（下载失败时支持一键重新下载） | 技术上极难实现，不会制作。 | #3069
 | 支持下载或安装资源时暂停下载 | 技术上极难实现，不会制作。 | #3069
 | 添加暗黑模式 | *“这个基本上要重新设计所有界面，工作量太大了，我猜我都不会做……” ——龙腾猫跃* | #131
 | Mod 管理允许选择使用多种排序方式 | 考虑到该功能可以使用 Windows 自带资源管理器进行排序，暂无必要在启动器侧实现。 | #2698
 | Mod 管理允许扫描子文件夹 Mod | 此功能已被移除 [^3]，但如果子文件夹名称为版本名则仍会读取并加载。对于 Quilt 加载器下识别子文件夹 Mod 功能正在处理。 | #811 #1098 #1536 #1784
 | 添加更多 Minecraft 远古版本 | 已有相关 Pull Request。 |  🔹 **#4555** <br> #3786
 | 添加不由 Mojang 发布的 Minecraft 版本 | 不会收录社区玩家制作的 Minecraft 版本（如：error422、alpha v1.2.3_03 等）。 | #2575
 | 添加云端账户、启动器内置社区、云端同步账户数据、云端同步隐藏主题、官网等 | 无法抵御攻击，不会制作任何有关云端账号的内容。 | #315 等 Issues
 | 支持隐藏主题迁移 | 考虑到隐私问题，不考虑支持导出此类信息。 | #760
 | 有关拓展隐藏主题、自定义主题、背景图片功能的 Issue | 备注：此类 Issue 大概率会因为必要性及优先级较低被拒绝，但不排除个别会被采纳，仅作参考。<br> *搜索关键词：毛玻璃、背景、透明、标题、隐藏主题、音乐、图标、暗黑、RGB、渐变、图标。* | #3202 #2216 #1487 #1653 #1242 #840 #791 #711 #562 #401 #131
 | 使用滑稽彩导致卡顿&掉帧&占用过大 | 无法解决或优化此类问题。 | #1575 #1590 #2336
 | 支持启动器字体自定义 | 会导致严重的 UI 适配问题，不考虑制作。 | #1724 #766 #366
 | 支持启动器开机自启动 | 不考虑在启动器内添加支持。 | #2896
 | 无法准确设置游戏分辨率 | 正在处理。 | #4654
 | 有关与 Minecraft 多人游戏服务器交互的内容 | 不会制作该功能。 | #829 #1993
 | 接入 ChatGPT、文心一言、Copilot、NewBing 等 AI 语言模型 | 不会制作该功能。 | #2791 #1557
 | 支持使用相对路径 | *“改这个那一大堆路径设置绝壁一周之内就会出来一大堆反馈让我加相对路径，想想都吓人，算了……” ——龙腾猫跃* | #1568 #1292 #1080
 | 游戏崩溃时加粗或突出窗口中 “而不是发送这个窗口的截图” 字样 | *“没救，侠客咋样都是侠客” ——龙腾猫跃* | #2153
 | 打开 PCL 时允许关闭此前已运行的 MC | 技术上难以识别一个 Java 进程是否为真正的 MC 进程，且必要性不大，不会制作。 | #1243
 | 开发简易版 PCL | 不会制作。<br> *搜索关键词：Lite、简易、简单、极简、轻量级、新手、萌新。* | #2330
 | 上架微软商店 | 不会制作该功能。 | #1278
 | 有关 “千万别点” 的 Issue | PCL **不会受理** 关于 “千万别点” 的 **任何 Issues**。 | #460 #398 #407 #677 #796 #1147 #1923
 | 添加内置 NBT 查看器/编辑器 | 超出启动器范畴，不会制作。 | #3321
 | 选中 PCL 文件并快速敲击 Enter 会导致 PCL 多开 | 无法正确检测，不会修复。 | #1372
 | 无法启动 LabyMod 客户端 | 为其版本 JSON 提供的文件大小有误所致，非 PCL 问题。 | #3225
 | 删除 Libraries 文件夹或其中的文件后补全文件失败 | PCL 无法在 Libraries 文件不全的情况下完成文件补全。 | #3698
 | 将 GitHub 链接替换为镜像站 | 代理源的安全性与稳定性欠佳，不会制作。 | #2879
 <!-- BUILD_FLAG:END PCL -->


### 难检反馈

 <!-- BUILD_FLAG:BEGIN Hard -->
 | 内容 | 解释 | 参考 |
 |--|--|--|
 | 因第三方组件引起的问题 | PCL 不会处理第三方造成的问题。 | *[Label:&nbsp;第三方](https://github.com/Hex-Dragon/PCL2/issues?q=label%3A%E7%AC%AC%E4%B8%89%E6%96%B9+is%3Aclosed)*
 | 因使用可编译开源版本导致的问题 | 因可编译版本可能经过了二次修改，因此此类版本造成的问题可能与 PCL 原版无关。| #3948
 | 因使用 32 位系统引起的问题 | 新版 Minecraft 已不支持 32 位系统，因此不会再额外为 32 位进行修复和调整。 | [#3649](https://github.com/Hex-Dragon/PCL2/issues/3649#issuecomment-2047054821)
 | 因系统问题无法打开 PCL | 系统原因，PCL 无法解决。<br> *搜索关键词：.NET、支持库、程序出现未知错误、显卡驱动、闪退、系统不完整。* | #2849 #2755 #2751 #2729 #2676 #2580 #2485 #2146 等 Issues
 | 调试模式性能损耗过大 | 个别问题，无法稳定复现。 | #365
 | Mod 下载详情页加载动画 UI 在加载后未能隐藏 | **[需要社区复现]** 需要社区给出稳定的复现方式。 <br> *搜索关键词：加载动画、加载图标、Mod 下载、列表、UI、隐藏、消失。* | #1624
 | 无法加载 Mod 图标 | 请检查您的网络环境，如无问题则请前往 Modrinth 或 CurseForge 网站内及 HMCL、BakaXL 内查看是否有图标，若均无图标，则该 Mod 作者未上传图标，非 PCL 问题。| -
 | 没有安装重复 Mod 却提示安装了重复 Mod | 部分 Mod 使用了相同的 Mod ID 导致 Mod 加载器误判为相同 Mod，请在安装 Mod 前仔细检查官方文档 / 百科确认可以同时安装后再安装。| #4376
 | 使用特定 Java 时无法结束或者取消启动 Minecraft | 由于部分 Java 会以很奇怪的方式运行 MC，并会再创建一个 Java 进程，导致 PCL2 无法分辨到底哪一个才是 Minecraft 进程，因此无法修复。 | #364
 | 内存优化后（或已使用内存过小时）已使用内存部分不显示具体数字 | 由于排版空间不够不予以显示，同时考虑到大部分玩家在内存占用极低时不会计较具体占用内存数，因此这是刻意的设计。 | #1924
 | 窗口最底部卡片展开时无动画 | WPF 的逻辑问题，技术上无法处理。 | #4739
 | 切换音乐时概率性切换提示与实际播放歌曲不符 | NAudio 的 Bug，技术上无法处理。 | #866
 | 切换音频设备后，音乐播放不会自动切换到新设备 | NAudio 的 Bug，技术上无法处理。 | #480
 | 播放音乐时提示线程执行失败：`NoDriver calling waveOutRestart` | NAudio 的 Bug，技术上无法处理。 | #1753 #2348
 | 启动游戏时出现弹窗报错：GLFW error 65543 | 检查是否使用了正确的显卡（或独立显卡）启动 PCL。 | #2215
 | 启动 Minecrat 1.7.10~1.12.2 游戏内无声音 | 此为 OpenAL 初始化失败所致，请在游戏启动后按下 F3+T 来重新初始化 OpenAL。 | #3779 [MC-9974](https://bugs.mojang.com/browse/MC-9974)
 | 因感染蠕虫病毒导致 PCL 崩溃或无法更新等 | *Collaborator 请注意，日志可见：文件名或文件夹名前含有 `cache`、`HD` 字样。* | #2964 #2970 #3204
 | 日志出现 `not xxx in java.library.path` | Java 不完整，非 PCL 问题，如果可能，请您自行准备 Java 而不是使用自动补全 Java 功能。 | #3496

 <!-- BUILD_FLAG:END Hard -->
 <!--参阅 #59，需要重新编写。
 | 无法更新 PCL（DNS） | 请按下 Win+X ，点击 Windows PowerShell（管理员），并输入如下命令 ```netsh interface ip set dns  "适配器名称" static 8.8.8.8```[^5]，如果您使用的是 **有线连接（网线）**，请将 **适配器名称** 替换为 **以太网**，如果您使用的是 **WiFi**，请将 **适配器名称** 替换为 **WLAN**，然后输入 ```nslookup raw.githubusercontent.com```，确认 **非权威应答** 的 **Addresses** 项的值不为 0.0.0.0、127.0.0.1、:::、:::1。 | #3505
 -->



### 预设主页
>
>[!IMPORTANT]
> 以下为 PCL2 内置的预设主页，均由第三方作者制作。
> 
> 如若以下自定义主页出现问题，**请通过下表提供的渠道向主页作者提交反馈，而不是向 PCL2 仓库提交 Issue**。

 | 主页名称 | 反馈地址 | 联网更新地址 | 作者 |
 |--|--|--|--|
 | Minecraft 新闻 | · [GitHub](https://github.com/Light-Beacon/PCL2-NewsHomepage/issues/new/choose) | · https://pcl.mcnews.thestack.top | @Light-Beacon
 | 简单主页 | · [GitHub](https://github.com/MFn233/PCL-Mainpage/issues/new/choose) | · https://raw.gitcode.com/MFn233/PCL-Mainpage/raw/main/Custom.xaml | @MFn233
 | 每日整合包推荐 | · [SodaMC](https://sodamc.com/31402-29042412.html) | · https://pclsub.sodamc.com | @wkea
 | Minecraft 皮肤推荐 | · [SodaMC](https://sodamc.com/45080-44052300.html) | · https://forgepixel.com/pcl_sub_file | @wkea
 | OpenBMCLAPI 仪表盘 Lite | · [GitHub](https://github.com/Mxmilu666/cloudflare-pcl-bmclapi/issues/new/choose) | · https://pcl-bmcl.milu.ink | @Silverteal <br> @Mxmilu666
 | PCL 主页市场 | · [GitHub](https://github.com/HomePlaza-Of-PCL2/Homepage-Market/issues/new/choose) | · http://pclhomeplazaoss.lingyunawa.top:27000/d/Homepages/JingHai-Lingyun/Custom.xaml | @JingHai-Lingyun
 | PCL 新闻速报 | · [GitHub](https://github.com/Joker2184/UpdateHomepage/issues/new) | · http://pclhomeplazaoss.lingyunawa.top:27000/d/Homepages/Joker2184/UpdateHomepage.xaml | @Joker2184
 | PCL 新功能说明书 | · [GitHub](https://github.com/WForst-Breeze/Whats-New-PCL2/issues/new) | · https://raw.gitcode.com/WForst-Breeze/WhatsNewPCL/raw/main/Custom.xaml | @WForst-Breeze
 | OpenMCIM 仪表盘 | · [GitHub](https://github.com/Hex-Dragon/PCL2/discussions/4906) | · https://files.mcimirror.top/PCL | @SALTWOOD
 | 杂志主页 | · [GitHub](https://github.com/Hex-Dragon/PCL2/discussions/4926) | · http://pclhomeplazaoss.lingyunawa.top:27000/d/Homepages/Ext1nguisher/Custom.xaml | @Ext1nguisher

<!-- 以下主页等待加入 PCL 预设
 | 历史上的今天 | · [GitHub](https://github.com/hsuchenghao/pcl-history-today-go/issues/new) | · https://pclnews.52chye.cn/custom.xaml | @hsuchenghao
 | 炽翎主页 | · [GitHub](https://github.com/YuShanNan/ChiLing-HomePage-PCL2/issues/new) | · http://samiuv.mcfuns.cn/PCL2/Custom.xaml | @YuShanNan
--> 


<details>
<summary>【附】如何优雅地解决问题&提交反馈？</summary>

### 我游戏崩了！急急急急急急

先别急，请导出并保存 PCL 输出的错误报告，首先尝试在相关 Minecraft 论坛、QQ 群（或 KOOK 群等相关 Minecraft 社群）、PCL2 仓库 Discussions 提问板块 **上传您的错误报告** 并描述您的具体情况。请注意，**不要仅上传 PCL 窗口的截图！不要仅上传 PCL 窗口的截图！不要仅上传 PCL 窗口的截图！** 也请在提问过程中尽可能保持 **平和友善的语气**，这会使您的问题得以更快解决。当游戏使用 PCL 启动或游玩过程中崩溃，而使用其他启动器启动或游玩时并未出现崩溃情况时，请在本仓库提交 Issue，并上传 PCL 日志及游戏崩溃报告、HMCL 启动脚本（如有）

如果您在求助时被指出需要提供 Mod 列表，可以在启动器中的 “启动前执行命令” 栏输入 `dir "{verindie}mods" /b | clip` 后重新启动游戏，Mod 列表就会被复制到剪贴板。

### 我想交反馈

#### 0. 在开始之前……

为了提高反馈处理效率，我们推荐您依照以下步骤来提交反馈。在沟通过程中，请保持平和友善态度，避免与他人产生言语冲突，这是不利于解决问题的。**请注意，重复反馈、无效反馈、优化建议、新功能提案无法获得活跃橙。**

#### 1. 重复反馈自检（重要）

在提交反馈前，请先确认您想提交的内容是否被他人提交，在 Issues 页面中的搜索栏搜索您想提交的内容的关键词。如：“支持识别和安装 Quilt”，您可以搜索 “Quilt” “加载器” “识别” “安装” 等关键词。在出现搜索结果后，在 “Open” 部分查看是否有相似 Issue，如没有，请单击 “Closed” 字样并再次检查是否有相似 Issue，如搜索结果过多，可以在搜索栏中添加 `label:忽略` 或 `label:"拒绝 / 放弃"` 来缩小检索范围。

#### 2. 反馈类型确认

完成后，单击 **New Issue** 按钮，根据列表各项提示，选择您要提交的 Issue 类型。**其中对于 Minecraft 崩溃，请见上条 “我游戏崩了！急急急急急急” 的描述后再提交 Issue。**

#### 3. 撰写反馈内容并提交信息（重要）

首先一一完成页面中出现的检查项，**确认无误后** 开始填写反馈内容。在编辑 Issue 标题时，请尽量保证标题 **简短且可以有效概括反馈内容**。如：

- ✔ Mod 管理选择 Mod 后下方按钮显示异常
  - 此标题明了地标明了问题出现位置及问题具体情况。
- ✔ 支持通过快捷键全选 Mod
  - 此标题清晰地表达了对于某内容的期望，并给出了可供参考的解决方案。
- ❌ 游戏崩了
  - 此标题……概括性极强……对……就……挺强的……就
- ❌ 5个建议
  - 请注意，不要一个 Issue 提交多个反馈内容，处理起来真的很头大。

完成上述步骤后，开始填写反馈内容正文部分，依照各部分提示清晰、明了、易懂地写出您的期望内容，如果可以，请写出可供参考的解决方案。

正文填写完毕后，请按照提示上传相关附件，包括但不限于：[Bug] PCL 日志、游戏日志、游戏崩溃报告、HMCL 启动日志、问题截图、复现视频等；[优化/新功能] 相关截图或视频。

> **💡 Tip: 开启调试模式复现问题**  
>
> 在反馈 Bug 时，我们推荐直接上传 **开启调试模式复现了问题的复现日志**，这通常会有利于解决该问题。  
若您尚不清楚如何开启调试模式，请开启 “设置 → 启动器 → 调试选项 → 调试模式” 后重启启动器即可。

#### 4. 后续处理及跟进工作

若您的反馈被初步确认，Collaborator 将会为您的 Issue 添加 `等待确认` label，如信息不足，请依照请求尽快完成信息补充，根据内容复现及相关信息获取难易程度，您需要**尽可能在两周内完成信息补充**，否则您的 Issue 将被超时关闭。但不必担心，若 Issue 关闭后您完成了信息补充，我们会再次进行确认，无误后会重新打开该 Issue。

在沟通过程中，请尽可能避免连续评论或多层引用评论，如果需要修改或补充您的陈述，可以通过单击右上角的三个点，选择 Edit 来编辑您的评论或反馈。在沟通过程中请尽可能**保持态度平和，避免出现过激言论**，如您对 Issue 处理结果不满意，可以继续在下方进行信息补充。

同时请注意，在沟通过程中请避免过多谈论无关内容或进行 [版聊](https://baike.baidu.com/item/%E7%89%88%E8%81%8A/403656)，尽管您可以对您发布的评论进行隐藏，**但当您发表无关内容时，已经对他人进行了不必要的打扰（因为该仓库有任何动态时 GitHub 会给关注了这个仓库的人发一次邮件）**，若无关内容过多，**该 Issue 将被锁定**。因此为了提高沟通效率，**请善用 Edit 编辑功能**，避免连续发布评论和发表无关内容。

</details>

<!-- BUILD_FLAG:BEGIN Footnote -->
[^1]:请注意，离线账号登录服务器本身违反 [Minecraft 最终用户协议](https://www.minecraft.net/zh-hans/eula) 提及的 [Minecraft 使用准则](https://www.minecraft.net/zh-hans/usage-guidelines) 的内容 ( 原文如此：*访问您的服务器：必须**只授予拥有 Minecraft 正规付费版本的用户*** ) ，请谨慎考虑。  
[^2]:i. 对于较老 Mod 搜索结果无法显示支持 Mod 加载器，此为早期 CurseForge 不支持设置选择 Mod 加载器导致；<br>ii. 对于输入搜索关键词无法搜索到指定 Mod 或搜索时出现无关 Mod，此为 API 问题；<br>iii. 如确认为 Mod 作者上传时的设置问题，例如错误地选择了不支持的版本、Mod 前置标记错误、译名错误等问题，请尝试联系 Mod 作者或 MCMod 百科页（仅译名问题）进行沟通确认。  
[^3]:由于 .minecraft/mods 文件夹下创建的子文件夹内的 Mod 不被 Mod 加载器（此为如 Forge、Fabric 类 Mod 加载器行为，非 PCL 行为）加载，因此在新版本中移除了此功能。  
[^4]:**▷▷▷ 请注意，Octo 开放不等价于 PCL 上线联机，具体信息以龙猫发布的消息为准，仅供参考。届时切勿散布任何未经相关启动器作者及服务提供方证实的信息。**  
[^5]:复制过程中，除适配器名称需要替换外，其他内容不可替换；除适配器名称外，其他部分不要包含中文字符。
<!-- BUILD_FLAG:END Footnote -->
