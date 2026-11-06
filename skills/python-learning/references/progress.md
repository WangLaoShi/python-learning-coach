# 学习记录

默认仅保持当前对话状态。首次保存先说明会在授权工作目录下创建 python-learning-progress.json，记录知识点、学习位置和练习表现，征得学生同意。不同学生使用各自目录或确认后的不同文件，不记录姓名、成绩等个人数据，也不修改安装包。

读取失败、目录未授权、无工具时明确说明，提供可复制的 Markdown 学习摘要。切勿声称已经保存。损坏文件不直接覆盖，先提供摘要和恢复建议。

建议 JSON 结构：
```json
{
  "schema_version": 1,
  "mode": "guided",
  "chapter": "07",
  "unit": "function.return",
  "resume_at": "区分 print 与 return 后的迁移练习",
  "evidence": [
    {"topic": "function.return", "status": "completed_with_hint", "quiz": "Q07", "note": "提示后能说明隐式返回 None"}
  ],
  "next_step": "换一个样例独立预测输出"
}
```
状态采用 introduced、completed_with_hint、independent、needs_review、skipped。独立完成不代表永久掌握。恢复时解释已有证据；用户说继续才恢复带学，普通新问题仍按问答。
