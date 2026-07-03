# BookSmart 文档管理工具

BookSmart 是一个桌面端文档管理工具，当前发布包包含主程序、前端静态文件、数据库迁移脚本和版本信息。首次运行后，程序会在本地自动创建用户数据目录。

## 版本信息

- 应用名称：BookSmart Document Manager
- 当前版本：v0.2.0
- 发布类型：桌面端
- 数据状态：发布包不包含用户数据

## 快速开始

1. 进入 `release` 目录。
2. 双击 `BookSmart.exe` 启动系统。
3. 程序启动后会自动打开浏览器页面。

## 目录结构

```text
release/
├── BookSmart.exe        # 主程序
├── Usetext.txt          # 使用说明
├── static/              # 前端页面文件
├── migrations/          # 数据库升级脚本
├── version.json         # 当前版本信息
└── data/                # 用户数据目录，首次运行后自动生成
```

## 数据存放

首次运行后，程序会在 `release` 目录下自动创建 `data` 文件夹。

所有文档、数据库和备份文件都会保存在 `data` 文件夹内。请不要删除该目录，否则可能导致数据丢失。

正式发布包默认不包含以下用户数据内容：

- `data/`
- `app.db`
- `uploads/`
- `backups/`

## 备份建议

建议定期在系统设置中执行数据备份。备份文件会保存在 `data/backups` 目录中。

## 更新说明

更新程序时，通常只需要替换以下内容：

- `BookSmart.exe`
- `static/`
- `migrations/`
- `version.json`

更新前请始终保留原有 `data` 文件夹。

## 关闭程序

关闭启动时出现的命令窗口即可停止服务。

如果浏览器页面无法访问，请重新双击 `BookSmart.exe` 启动。


网盘分享的文件：booksmart发布版.zip 链接: https://pan.baidu.com/s/1EztUrwWOgo6kXGaekzzkKw 提取码: begx 复制这段内容后打开百度网盘手机App，操作更方便哦