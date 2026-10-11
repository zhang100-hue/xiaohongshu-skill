# 小红书双账号运营 Skill v1.0

这是一套可落库的原创工作包：A 做简约治愈漫画，B 做复杂排版模板与原创视觉设计；分别增长、归档与评估商业化。当前没有接入真实小红书账号、后台数据或发布权限，目录里的 `EXAMPLE` 只是占位。旧草稿包位于本地 `output/xiaohongshu-skill-v0.2.0/`，本包不声称继承其真实账号数据。

## 文件

- `.agents/skills/xiaohongshu-dual-ops/SKILL.md`：Codex 入口。
- `agents/openai.yaml`：桌面技能显示名与默认提示。
- `references/`：分账号增长、漫画、视觉设计、作品集版权、发布合规。
- `templates/`：单篇制作卡和周复盘。
- `config/accounts.json`：两个内部账号配置，真实 ID 留空。
- `portfolios/comics/` 与 `portfolios/visual-design/`：独立作品集索引与占位样例。
- `SOURCES.md`：来源、许可与核验状态。

## 在桌面 Codex 使用

1. 将本包作为工作目录打开。Codex 会从仓库/当前目录的 `.agents/skills` 发现 Skill；如未出现，重启 Codex。也可将技能文件夹复制到用户级 `$HOME/.agents/skills/`。不要仅把 ZIP 原样放进技能目录。参见 [OpenAI Skills 官方文档](https://learn.chatgpt.com/docs/build-skills)。
2. 在聊天中输入：`用 $xiaohongshu-dual-ops 为 A 做 3 条漫画选题和首篇分镜`；B 可说：`用 $xiaohongshu-dual-ops 为 B 做一套可编辑简历案例的内容简报`。
3. 填写 `config/accounts.json` 中真实账号 ID（仅在本地保存；公开仓库勿提交个人信息），提供过往笔记和后台数据。按制作卡审核图片、文字、版权与平台标识后，再由你手动发布。
4. 每件作品按作品集规则建目录、填权利清单和索引。每周分别复盘 A/B，真实链接和指标由你提供或授权读取。

## 后续建议开启的能力与权限

|能力|用途|建议|
|---|---|
|本 Skill|双账号工作流|先在该工作目录启用，保持自动发现|
|`skill-creator`|以后修改运营规则|按需调用，非每天必开|
|`imagegen`|A 漫画与 B 概念视觉的位图制作|按单篇使用；检查生成内容标识与素材授权|
|`presentations`、`documents`、`pdf`|B 的 PPT、简历文档和 PDF 交付|只有生产相应文件时使用|
|`spreadsheets`|运营指标、选题表和作品索引|有表格数据时使用，拒绝编造数据|
|GitHub 连接|版本管理、备份与审阅|只给目标仓库必要权限；公开仓库不存账号凭证、客户私料和未授权素材|
|文件写入|生成草稿与作品集|限定在工作目录；不要扩展为全盘权限|
|网络/浏览|查最新规则、授权和竞品公开信息|按需开启；不为日常制作常开全网络命令权限|
|小红书账号连接/自动化|读取数据或发布|当前无需开启。将来若启用，先确认工具来源、平台许可和每次外部动作授权|

桌面 Codex 的工作区写入、网络与审批是独立控制，默认工作区写入模式下命令网络受限；依需要开最小权限。参见 [OpenAI Agent approvals & security](https://learn.chatgpt.com/docs/agent-approvals-security)。本包不要求关闭沙盒或自动审批。

## 商业化使用

作品集先作为展示和版权台账。满足平台当日权限、稳定作品质量与实际询盘后，A 优先评估合集/衍生/角色授权，B 优先评估模板/素材包/定制设计。`references/accounts-growth.md` 里的观察门槛只是内部实验建议，不是平台准入规则或收益保证。
