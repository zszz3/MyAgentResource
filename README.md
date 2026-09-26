# AgentRecall 团队资产

此仓库由 agentrecall init 初始化。团队资产在 Git 中共同维护，项目选择需要的资产安装到本地。

## 目录

- agentrecall.json：AgentRecall 资产清单。当前支持 Skills 和工作配置。
- skills/：每个 Skill 使用独立目录和 SKILL.md，并在清单 skills 中登记 id 与 path。
- rules/、docs/、env/、members/：参考 TeamAI 的目录组织预留，当前不会自动分发或上传成员信息。请勿提交密钥。

## 使用

在 AgentRecall V2 设置中连接团队；进入团队后创建项目并关联本地 Git 目录，再手动同步和选择安装。CLI 也可使用 team enable、project add --team、team sync。初始化不会自动开启团队功能、安装 Hook 或上传 Session。

## 添加 Skill

创建 skills/review/SKILL.md，YAML frontmatter 包含 name: review 与非空 description，然后在 agentrecall.json 的 skills 中添加 {"id":"review","path":"skills/review"}。提交并推送后，团队成员可手动同步、预览和安装。
