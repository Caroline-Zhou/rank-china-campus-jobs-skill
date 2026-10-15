# 单一事实源与读取路由

工作区根目录：

`C:\Users\Caroline\Documents\Codex\2026-08-10\https-github-com-madslorentzen-ai-job`

每次使用本 Skill 时，按任务读取以下文件；使用 UTF-8：

1. 始终读取 `.claude/skills/job-application-assistant/01-candidate-profile.md`：候选人经历、教育、技能与事实边界。
2. 始终读取 `.claude/skills/job-application-assistant/04-job-evaluation.md`：资格门槛、入职门槛、评分权重与职业方向。
3. 抓取官网时读取 `.claude/skills/job-application-assistant/09-web-research.md`：信任边界、官网优先和抓取失败升级顺序。
4. 需要全网主动找岗或去重时读取 `.claude/skills/job-scraper/SKILL.md`；用户只给单家公司官网时不要为了形式运行无关门户。
5. 读取根目录 `CLAUDE.md` 获取持续授权、市场偏好和工作簿总规则；若它与分项方法文件冲突，以更具体、版本更新的分项文件为准，并指出冲突。

母工作簿：

`C:\Users\Caroline\Documents\Codex\2026-08-10\https-github-com-madslorentzen-ai-job\work\workflow-audit\周宛瑜_AI求职岗位追踪.xlsx`

交付同步副本：

`C:\Users\Caroline\Desktop\Path\AI agent\周宛瑜_AI求职岗位追踪.xlsx`

始终优先编辑母工作簿，验证后再同步到桌面路径。若两者时间或内容不一致，先比较并以较新的有效版本为基础，避免覆盖用户的新改动。

投递状态属于动态事实，只从用户最新消息和现有工作簿读取，不固化在本 Skill 中。不得让静态 Skill 覆盖用户后来确认的状态。
