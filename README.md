# MirrorMind
🌇 MirrorMind（镜中我）, 你可以把它当成一个心灵窗口

---

## 🧱 核心模块概览

| 模块名     | 描述                           |
| ------- | ---------------------------- |
| 用户系统    | 注册、登录、JWT 鉴权                 |
| 日志记录    | 用户每天写点什么（日志 / 情绪 / 问答）       |
| AI 分析模块 | 调用 OpenAI 识别情绪、提取关键词、生成建议    |
| 自我镜像报告  | 汇总近 7 天 / 30 天内容，输出视觉图表与总结文字 |
| 可视化反馈   | 图表展示：情绪趋势、关键词云、成长建议等         |

---

## 🗂 技术栈

* **前端**：Nuxt 3 + Tailwind CSS + Pinia + Chart.js
* **后端**：Nuxt Server API (或 Express) + Prisma ORM
* **数据库**：PostgreSQL（或 MySQL）
* **AI 模块**：OpenAI API（gpt-4o 模型优先）
* **部署**：Vercel (前端) + Railway / Supabase / Render (数据库 + API)

---
