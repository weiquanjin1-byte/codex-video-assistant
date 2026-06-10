# AI Video Content Assistant Agents

## 目标

本目录定义 AI 视频剪辑助手的多 Agent 协作系统。每个 Agent 只负责一个清晰环节，最终由 `compliance-review-agent` 做合规把关。

本目录适合公开发布，因为它只描述协作流程和安全边界，不包含 API Key、token、Cookie、账号信息、私人 evidence 原始记录或未授权素材。

## Agent 清单

| Agent | 职责 |
|---|---|
| `trend-research-agent.md` | 研究公开热点，判断可视频化和风险 |
| `script-writing-agent.md` | 将热点或主题转成视频脚本和分镜 |
| `copywriting-agent.md` | 生成标题、封面、发布正文、标签和评论引导 |
| `voice-selection-agent.md` | 选择配音风格、语速、停顿和重音 |
| `bgm-selection-agent.md` | 选择 BGM 方向并标记授权风险 |
| `editing-plan-agent.md` | 生成时间轴、镜头、字幕、转场、导出和最小成片步骤 |
| `aesthetic-review-agent.md` | 使用 `aesthetic-score.md` 做审美评分和优化 |
| `compliance-review-agent.md` | 检查隐私、版权、抄袭、造假、授权和平台规则 |

## 协作流程

1. `trend-research-agent` 找热点。
2. `script-writing-agent` 生成脚本。
3. `copywriting-agent` 生成标题、封面、发布文案。
4. `voice-selection-agent` 选择配音风格。
5. `bgm-selection-agent` 选择 BGM 方向。
6. `editing-plan-agent` 生成剪辑执行表。
7. `aesthetic-review-agent` 评分和优化。
8. `compliance-review-agent` 最终合规检查。

## 协作规则

- 每个 Agent 只能输出自己职责范围内的内容。
- 涉及授权、隐私、平台规则、热点真实性时，必须交给 `compliance-review-agent`。
- 热点只能作为选题参考，不能直接作为未经验证的事实。
- P0 原型只能用于内部测试，不得发布。
- 无法访问平台或无法验证数据时，必须说明无法访问或待验证。

## 必须遵守的合规边界

- 不抓取个人隐私。
- 不绕过平台限制。
- 不伪造热点数据。
- 不使用未授权 BGM、素材、字体、音效、图标或声音。
- 不混入其他项目数据。
- 不把未经验证的平台趋势写成事实。
- 热点研究只能使用公开、授权或用户提供的数据源。
- BGM、素材、字体、配音、音效和图标在使用前必须确认授权。
- 本项目是辅助创作工具，不保证自动生成内容一定适合发布。
