# LaunchHome:把启动台带回 macOS 26

![LaunchHome](https://launchhome.app/og/og-zh.jpg)

苹果在 macOS 26 (Tahoe) 里移除了经典的启动台。F4 和捏合手势现在打开的是 Spotlight 的「应用程序」视图——能搜索,但没有分页、没有文件夹、不能自己排顺序。对用惯了启动台的人来说,这半个屏的图标网格,是每天要按几十次的肌肉记忆。

**LaunchHome** 就是为此而做的:用纯原生 AppKit 把多页启动台完整带回 macOS 26 / 27——分页网格、拖拽整理、文件夹、拼音搜索、F4 一键呼出,以及你熟悉的那套手感。

- **官网**:<https://launchhome.app/>
- **直接下载**:<https://dl.launchhome.app/LaunchHome.dmg>(约 2.7 MB,Developer ID 签名并经 Apple 公证)

## 它能做什么

**熟悉的启动台,一颗不缺**

- 全屏图标网格,触控板横滑翻页、滚轮、方向键、页点点击,六种翻页动画(滑动 / 淡入淡出 / 缩放 / 立方体 / 翻转 / 层叠)
- 拖拽重排实时跟手;拖到屏幕边缘自动翻页;拖到一个图标上建文件夹;从文件夹拖出;空位自动补齐
- 弹层式文件夹,点击标题即重命名,成员分页
- 运行中的应用名下有小圆点指示;按名称 / 最近使用 / 使用频率排序
- 第一次运行可一键**导入旧系统启动台的布局**(分页、文件夹、顺序原样还原,前提是这台 Mac 上还留着旧数据),也可以按类别自动归类整理

**搜得快,才是启动台的意义**

- 打开即打字:中文名、全拼(`weixin`)、首字母(`wx`)、bundle ID 都能搜
- 输入算式直接出结果(`198*0.85=`),回车即复制
- Enter 启动第一个结果,Esc 逐层退出

**不止是启动台**

- 顶部小组件:计算器、时钟日历、剪贴板历史(仅存内存,绝不落盘)
- 网格里除了应用,还能放文件、网址、快捷指令和工作流脚本
- 每个应用可自定义图标、重命名显示名、彻底卸载(扫描并清理 `~/Library` 残留)
- ⌘/⇧ 点击多选,批量隐藏、移除、卸载
- 自定义应用来源目录、自定义行列数、视频壁纸、8 种界面语言(简/繁中文、English、日本語、한국어、Français、Deutsch、Español)
- 布局随时导出备份,读取失败的布局文件会被挪开保存而不是覆盖

**呼出方式随你**

- F4(系统 Carbon 热键,**无需辅助功能权限**);冲突时可录制任意组合键
- 触控板双指张开呼出、四指捏合收起;鼠标触发角;菜单栏图标;开机自启

## 性能与隐私

在一台 Apple Silicon 的 Mac 上实测:首次打开约 181 ms,之后每次复开不到 5 ms,稳态内存约 99 MB。图标按需渲染,空闲不占资源。

LaunchHome 不含任何统计或追踪代码。布局、设置和小组件数据全部留在本机;剪贴板历史只存内存、从不写盘。试用与激活时仅向服务器发送硬件 UUID 加盐后的 SHA-256 哈希,用于标识设备,不暴露原始信息。授权令牌在本地验签,**离线也能正常使用**。

## 价格

| | |
|---|---|
| 试用 | 全功能免费试用 **7 天**,无需注册 |
| 买断 | **¥38**(国内,微信支付) / **US$9.9**(海外),无订阅 |
| 授权范围 | 一份授权可激活 **5 台 Mac**,1.x 版本更新全部免费 |
| 退款 | **14 天**无理由退款 |

- **国内购买**:<https://launchhome.app/zh/buy>(微信扫码)
- **海外购买**:[官网价格区](https://launchhome.app/#pricing) / [Creem 结账页](https://www.creem.io/payment/prod_59Tt3ZvqiKMUVrRUYgMMhu)
- 授权码丢了?输入购买邮箱即可[找回](https://launchhome.app/zh/)

## 下载与安装

1. 下载 [LaunchHome.dmg](https://dl.launchhome.app/LaunchHome.dmg)(macOS 26 Tahoe / macOS 27,Apple Silicon 与 Intel 通用)
2. 把 LaunchHome 拖进「应用程序」,打开,按 F4
3. 旧 Mac 升级上来的?在搜索栏右侧菜单里选「导入系统启动台布局」,原来的分页和文件夹一键还原


## 关于工程

LaunchHome 是一个纯原生 AppKit 项目,**零第三方依赖**,代码分两层:纯逻辑核心(模型 / 网格几何 / 布局持久化 / 拼音索引 / 授权验签)和 AppKit 界面层。


## 链接汇总

| | |
|---|---|
| 官网(中文) | <https://launchhome.app/zh/> |
| Website (English) | <https://launchhome.app/> |
| 下载 | <https://dl.launchhome.app/LaunchHome.dmg> |
| 购买(国内) | <https://launchhome.app/zh/buy> |
| 「macOS 26 怎么找回启动台」指南 | <https://launchhome.app/zh/launchpad-macos-26/> |
| 更新日志 | <https://launchhome.app/changelog/> |
| 隐私政策 | <https://launchhome.app/privacy/> |
| 退款政策 | <https://launchhome.app/refund/> |
| 最终用户许可协议 | <https://launchhome.app/terms/> |
| 联系我们 | <support@launchhome.app> |

---

