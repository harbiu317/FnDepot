# FnDepot

harbiu317 的飞牛 NAS（fnOS）第三方应用源仓库，遵循 [FnDepot 应用源构建规范](https://github.com/EWEDLCM/FnDepot)。

## 订阅本仓库

在飞牛 NAS 上安装 FnDepot 客户端后，添加以下源地址即可：

```
https://github.com/harbiu317/FnDepot
```

## 应用列表

| 应用 | 说明 | 平台 | 版本 |
|---|---|---|---|
| [图床 PicHub](pichub/) | 自托管图床，多云存储 / 相册 / API Token | x86 | 1.0.16 |
| [Tunebox](tunebox/) | 多平台聚合音乐搜索下载工具 | x86 | 1.0.1 |
| [LX Music Player](lxserver/) | 聚合多平台音乐搜索与在线播放 | x86 | 1.0.4 |
| [飞牛终端](terminal/) | Web SSH 终端，多标签、SSH 连接管理 | x86 | 1.0.1 |

## 仓库结构

```
FnDepot/
├── fnpack.json          # 全局应用索引（FnDepot 客户端读取此文件）
├── pichub/              # 图床 PicHub
│   ├── ICON.PNG
│   ├── README.md
│   └── Preview/         # 预览截图
├── tunebox/             # Tunebox
│   ├── ICON.PNG
│   ├── README.md
│   └── Preview/
├── lxserver/            # LX Music Player
│   ├── ICON.PNG
│   ├── README.md
│   └── Preview/
└── terminal/            # 飞牛终端
    ├── ICON.PNG
    ├── README.md
    └── Preview/
```

fpk 安装包通过 `download_url` 字段指向各应用源仓库的 GitHub Release，避免本仓库膨胀。
