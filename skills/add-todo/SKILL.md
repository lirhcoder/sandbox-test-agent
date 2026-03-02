---
name: add-todo
description: 创建一个新的待办事项
trigger: 当用户要求添加、创建待办事项时
---

# 执行步骤

1. 从用户消息中提取待办事项的标题和描述
2. 生成 slug（英文小写，短横线连接）
3. 获取当前日期（YYYY-MM-DD 格式）
4. 在 `app-memory/todos/` 目录下创建 `{date}-{slug}.md` 文件
5. 文件内容格式：

```markdown
---
status: pending
priority: medium
created: {date}
---

# {标题}

{描述}
```

6. 向用户确认待办事项已创建
