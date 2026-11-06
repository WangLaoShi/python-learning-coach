# Python 学习教练 · WorkBuddy 试用包 0.1.0

默认随问随答，明确说“带我学习第 N 节”后才进入带学。覆盖基础、必备能力、拓展、学习路径、小测、错误解答。不需要百炼 API Key，不需要启动此前的教程网页；使用 WorkBuddy 自身的模型、工具与授权。

## 推荐安装：客户端创建专家

官方客户端流程是“专家·技能·连接器 → 我的专家 → 创建专家”，由创建对话配置。官方未承诺所有客户端版本都有 ZIP 直接导入按钮。请使用以下方式：

1. 解压 ZIP 到你愿意授权 WorkBuddy 读取的文件夹，保留隐藏的 `.codebuddy-plugin` 目录。
2. 在 WorkBuddy 打开/授权这个解压目录。进入“我的专家 → 创建专家”。
3. 复制本包 `INSTALL-PROMPT.md` 中的创建请求到对话，并按实际提示完成配置。该请求要求内置管理工具读取配置、Agent 与关联 Skill；不要仅上传一份讲义就认为全部配置已加载。
4. 创建后，检查是否已关联 `python-learning` 技能。如果当前版本无法直接从专家包关联本地技能，可在技能界面使用本地技能导入（以实际入口为准）；或让创建工具使用本包技能目录完成关联。不能导入时，明确报告不支持的步骤，不自动修改未知内部数据库。
5. 召唤“Python 学习教练”，先问“print 和 return 有什么区别？”，再试“带我学习第 7 节”。可用 acceptance/cases.md 验收。

如果当前客户端无法读取本地包，可把 Agent 文件正文粘贴为专家工作要求，配套技能单独导入/提供。此降级方式的资料读取和持久进度取决于实际工具授权，不保证等同完整安装。

## 专家包格式 / 开放平台

`.codebuddy-plugin/plugin.json`、`agents/`、`avatars/`、`skills/` 按官方专家包规范组织，ZIP 内直接放这些目录，无多余外层目录。开放平台支持提交专家包，但涉及开发者身份、审核和发布，不是个人本地试用的必要步骤。本次没有提交或公开发布。

作者名称为“Python Course”，作者邮箱为 `wangjianxu@aliyun.com`。提交市场前请核对作者信息、授权与平台要求。

## 试用指令

- 解释为什么 input() 的结果不能直接加 5。
- 带我学习第 2 节：变量与类型。
- 暂停带学，直接给我完整答案。
- 针对循环出一道小测，先不要给答案。
- 这段代码没有报错，但平均分不对，帮我定位。
- 画出字典、JSON 和 API 的知识关系。
- 我想保存学习进度，请先说明保存位置和内容。

## 包内内容

- `agents/python-learning-coach.md`：专家角色和模式切换。
- `skills/python-learning/SKILL.md`：资料与工作流入口。
- `skills/python-learning/references/`：17 节教材、路径、小测、答案、教学、排错与记录规范。
- `skills/python-learning/examples/grade_report.py`：标准库综合示例。
- `acceptance/cases.md`：行为验收案例。

进度只有得到学生同意且目录获授权后才保存到学习工作目录，不写专家安装目录。不自动执行学生代码、不自动安装依赖。不假装记得跨会话进度或实际运行过代码。

## 验证边界与来源

本包完成本地配置结构、资源引用、技能格式、ZIP 完整性及综合示例验证；尚未在你的 WorkBuddy 客户端中实际安装、运行专家或通过开放平台审核。题目与教学规则的实际效果以试用为准。

教程改编自 [Aliyun-Python](https://github.com/WangLaoShi/Aliyun-Python) 仓库中的 `v2610/01-Python一篇概全.md`；沿用该项目的 Python 教学资料脉络。未附带第三方教程全文、账号凭据或学生个人数据。头像为原创几何书本图标。

官方参考（2026-11-06 核对）：
- 专家包规范：https://open.workbuddy.cn/docs/expert
- 客户端创建：https://www.workbuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Expert-Center
