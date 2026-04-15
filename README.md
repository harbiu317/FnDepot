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
| [图床 PicHub](pichub/) | 自托管图床，多云存储 / 相册 / API Token | x86 | 1.0.14 |
| [Tunebox](tunebox/) | 多平台聚合音乐搜索下载工具 | x86 | 1.0.0 |
| [飞牛终端](terminal/) | Web SSH 终端，多标签、SSH 连接管理 | x86 | 1.0.0 |

## 仓库结构

```
FnDepot/
├── fnpack.json          # 全局应用索引
└── tunebox/             # 应用目录
    ├── ICON.PNG
    ├── README.md
    └── Preview/         # 预览截图
```

fpk 安装包通过 `download_url` 字段指向各应用源仓库的 GitHub Release，避免本仓库膨胀。
