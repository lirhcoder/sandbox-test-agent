---
name: list-todos
description: 列出所有待办事项
trigger: 当用户要求查看、列出待办事项时
---

# 执行步骤

1. 读取 `app-memory/todos/` 目录下所有 `.md` 文件
2. 解析每个文件的 frontmatter（status, priority, created）和标题
3. 按创建日期倒序排列
4. 以表格或列表形式展示给用户：
   - 标题
   - 状态（pending/done）
   - 优先级
   - 创建日期
5. 如果没有待办事项，提示用户可以用 add-todo 创建
