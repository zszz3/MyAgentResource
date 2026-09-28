# MyAgentResource

供 AgentRecall 团队空间使用的共享资产库。

## 资源

- **11 个 DSH Skills**：代码审查、提交检查、CI 稳定性、性能分析、代码简化、文档、客户端 UI 规范和配套 Agent Notes 维护。
- **2 份文档**：[DSH 技能使用说明](docs/dsh-resources.md)、[性能验证清单](docs/performance-checklist.md)。
- **1 份共享指令**：[团队开发约定](rules/team-development.md)。

## 使用

在 AgentRecall V2 设置中连接本仓库并启用团队，在团队空间浏览资源。接入工作目录、选择客户端后，点击「同步团队」统一更新。不会自动上传会话或执行 Skill 中的命令。

DSH 前缀技能保留 DeepSeek Harness 的工程约束，使用前核对当前工作目录与依赖；它们不能替代其他仓库自己的规则。完整范围和依赖见使用说明。

## 维护

agentrecall.json 是版本 4 资产清单。Skills 放在 skills/，共享指令放在 rules/，普通文档放在 docs/。MCP 与公共 Env 可按清单格式登记；密钥只保存本机变量引用，不提交实际值。

来源与许可：[第三方说明](THIRD_PARTY_NOTICES.md)、[逐文件来源记录](sources/dsh-skills.json)。每个 Skill 内也附有许可和固定版本的上游链接，便于单独分发。
