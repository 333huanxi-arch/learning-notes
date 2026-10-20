# 读书学习笔记 (Learning Notes)

> 用 GitHub + Markdown 记录每天读书与学习的成长轨迹。

## 这是什么

一个用纯文本（Markdown）管理的读书 / 学习笔记仓库。每本书单独一个目录，每天的学习内容写成一篇「日记式」笔记，全部交给 Git 做版本管理——自动保留每次修改的历史，永远不会丢。

## 目录结构

```
learning-notes/
├── README.md              # 本文件：项目说明 + 总索引
├── .gitignore             # 忽略不需要提交的文件
├── templates/             # 可复用的笔记模板
│   ├── daily-note.md      # 每日学习日志模板
│   └── book-note.md       # 单本书总览模板
├── books/                 # 每本书一个目录
│   └── example-book/      # 示例书
│       ├── README.md      # 这本书的总览（进度/评分/总结）
│       └── notes/         # 按日期记录的每日笔记
│           └── 2026-10-20.md
└── daily/                 # 跨书的每日汇总（可选）
    └── 2026-10-20.md
```

## 命名约定

- 书名目录用小写英文 + 连字符，例如 `thinking-fast-and-slow`、`深度工作`。
- 每日笔记文件名统一用 `YYYY-MM-DD.md`，方便按时间排序和检索。

## 怎么开始

1. 在 GitHub 新建一个仓库（建议公开，方便回顾与分享）。
2. 把本目录推上去（见下方命令）。
3. 复制 `templates/daily-note.md` 到 `books/<书名>/notes/YYYY-MM-DD.md` 开始记录。

## 常用命令

```bash
git add .
git commit -m "📖 2026-10-20 学习笔记"
git push
```

## 进阶玩法

- **总索引**：在 `README.md` 里维护一个「已读 / 在读」书单，链接到各书目录。
- **GitHub Pages / Docsify**：把仓库变成一个在线读书站，手机也能看。
- **Issues / Projects**：用 Issue 跟踪「想读清单」和「待思考问题」。
- **自动化**：用 GitHub Actions 每天自动生成当日空白笔记模板。
