# quanttide-profile-of-health-management
量潮健康管理档案

## 概述

本仓库收录健康管理场景下的**标准化测评量表档案**（profile），每个量表一份 Markdown 文档，以 YAML header 标注量表的**功能定位**（function）与元数据，供产品、开发直接引用。

## 量表索引

| 文档 | 量表 | 功能 | 题量 | 授权 |
|------|------|------|------|------|
| `scales/mini-ipip.md` | Mini-IPIP | 压力倾向基线（大五人格） | 20 | 公共领域 |
| `scales/pss-4.md` | PSS-4 | 近期压力感知 | 4 | 公共领域 |
| `scales/cbi.md` | CBI（哥本哈根倦怠量表） | 职业倦怠筛查 | 19 | 公共领域 |

## 组合使用方案

- **日常追踪（季度/半年）**：Mini-IPIP + PSS-4 —— 稳定基线 + 近期变化，判断"性格使然还是环境突变"
- **深度筛查（年度/触发式）**：Mini-IPIP 情绪稳定性与 PSS-4 双高时，追加 CBI 诊断职业倦怠

## 文档规范

每个量表文档必须包含 YAML header，关键字段：

| 字段 | 含义 |
|------|------|
| `function` | 功能定位（本仓库的核心标注字段） |
| `role` | 角色：核心工具 / 专项补充 / 深度筛查 |
| `items` | 题量 |
| `items_status` | 题目清单状态（complete=已含官方核对完整题目） |
| `dimensions` | 维度列表 |
| `response_scale` | 作答刻度 |
| `scoring` | 计分方式 |
| `judgment` | 判读标准 |
| `frequency` | 建议追踪频率 |
| `license` | 授权条款 |

## 合规底线

所有量表结果输出处须显著标注：**"本测试结果仅供参考，不构成医疗诊断"**。
