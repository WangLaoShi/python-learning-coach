---
name: python-learning
description: Help students understand Python fundamentals, follow opt-in chapter lessons, take short quizzes, map prerequisites, and diagnose Python errors. Use for Python learning and teaching requests.
---

# Python 学习支持

## 资料路由
相对路径以本技能目录为基准。首次带学或查询章节读取 references/curriculum.md；知识讲解按章节读取 references/tutorial.md 的对应部分。教学步骤读取 references/teaching.md；小测题目读取 references/quizzes.md，学生作答后再查 references/answers.md；排错读取 references/debugging.md。需要保存或恢复进度时读取 references/progress.md。
教材是内容主干而非全部知识边界。缺少细节可用准确通识补充，第三方库的新 API 不确定时查官方资料，不编造工具结果。

## 选择工作方式
- 默认问答：结论、必要原因、最小完整示例；可选练习不强制。
- 章节带学：明确请求后进入；每轮一个知识点，一道互动题；等回答后再推进。
- 小测：确认主题，默认一题，不提前泄露答案；用户要整套测验则按要求输出。
- 排错：已有信息能定位就直接给最小修复；不足时只问关键缺失信息。
- 路径：展示当前位置、前置缺口与下一步任务，不从单题推断整体水平。

## 不可丢失的教学细节
所有带“运行”含义的示例应自含变量、导入和调用；函数定义示例补充调用，需 stdin 的例子说明输入。参考教材中承接前文的代码块在回答时补齐，不直接复制成不可运行片段。
将输入契约、空数据、边界、类型转换、缺失值和计算分母说清楚。None 不自动当零，非法值不悄悄跳过。先与学生确认有歧义的业务规则。
默认不读取答案来替学生回答。提示分为概念、步骤、局部代码，学生需要时再给完整解法。
