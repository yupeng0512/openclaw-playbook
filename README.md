# OpenClaw Playbook

> OpenClaw 高价值使用场景与商业化落地方案手册

## 这是什么

[OpenClaw](https://github.com/openclaw/openclaw) 是 2026 年增长最快的开源 AI Agent 框架（234k+ GitHub Stars），能在本地运行自主智能体，连接 LLM 执行真实世界任务。

本仓库系统性地整理了 OpenClaw 的**高价值使用场景**和**可落地的实施方案**，目标是为后续的商业化落地提供扎实的调研基础和行动指南。

## 调研数据来源

| 来源 | 说明 |
|------|------|
| [OpenClaw 官方 Showcase](https://docs.openclaw.ai/zh-CN/start/showcase) | 社区真实项目展示 |
| Discord #showcase | 2,963 条消息, 922 位独立开发者 (2026.01-02) |
| ClawHub 技能市场 | 5,705 注册技能, 2,868 精选, 1.5M+ 下载 |
| [awesome-openclaw-usecases](https://github.com/hesamsheikh/awesome-openclaw-usecases) | 社区使用案例精选 (10.7k ⭐) |
| [awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) | 社区技能精选集 (21.6k ⭐, 2,868 Skill) |
| SoniaIA 社区分析报告 | 14 个 Agent 生产运行经验 |
| Medium / Dev.to / 技术博客 | 深度技术案例与教程 |
| Twitter/X 高赞内容 | 社区实战分享 |

## 文档目录

### 核心调研

- [使用场景与落地方案调研报告](docs/research-report.md) — 完整调研报告，12 大场景分类 + 优先级排序 + 2,868 Skill 生态概览
- [优先级矩阵](docs/priority-matrix.md) — 场景优先级速查表

### 落地指南（规划中）

- `docs/guides/` — 各场景的详细落地教程（含配置、架构图、踩坑记录）
- `docs/security/` — 安全加固与企业级部署方案
- `docs/case-studies/` — 社区标杆案例深度解析

## 优先级总览

| 优先级 | 分类 | 推荐原因 |
|--------|------|----------|
| **P0** | 个人助理（早间简报/邮件/日历/CRM/健康） | 落地最快、ROI 最高、社区验证最多 |
| **P0** | 开发者工作流（PR 审查/CI-CD/n8n/自愈服务器） | 原生优势、自动化程度高 |
| **P1** | 浏览器自动化（价格监控/数据采集） | 内置能力、无需额外工具 |
| **P1** | 智能家居（Home Assistant） | 成熟插件、20 分钟部署 |
| **P1** | 企业业务自动化（电商/发票/多渠道客服） | 高 ROI、已有生产验证 |
| **P1** | 调研与市场分析（RAG 知识库/财报/MVP 工厂） | 商业价值高、Skills 丰富 |
| **P2** | 多智能体编排 | 前沿但复杂，需架构经验 |
| **P2** | 金融交易 | 高价值但高风险 |
| **P2** | 内容创作/社交媒体（内容工厂/信息聚合） | 实用但平台限制多 |
| **P2** | 知识管理与记忆 | 长期价值高 |
| **P2** | 自主项目管理（STATE.yaml/目标驱动） | 提升 Agent 自主性 |
| **P3** | 语音与电话 | 前沿探索阶段 |

## 技术栈关键数据

- **社区首选模型**: Claude (Opus/Sonnet) 216 次提及 > Codex 59 > GPT 48 > 本地模型 127
- **首选消息渠道**: Telegram (92 次提及) > Discord > WhatsApp > Slack
- **硬件**: Raspberry Pi (174 次提及) 是"意外硬件冠军"
- **核心自动化机制**: Cron Job（定时任务） + Heartbeat（心跳检测） + Webhook（事件触发）

## 生态安全警告

ClawHub 5,705 个注册技能中，约 **48.2% 被过滤**（垃圾/恶意/重复），其中 **6.9%（396 个）确认含恶意代码**。安装任何第三方 Skill 前务必审查源码并查看 VirusTotal 报告。详见 [调研报告 - 安全章节](docs/research-report.md#安全风险)。

## 贡献

欢迎提交 Issue 和 PR，分享你的 OpenClaw 落地经验。

## License

MIT
