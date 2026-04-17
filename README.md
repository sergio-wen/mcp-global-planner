# @gloryfham/mcp-global-planner

荣耀全球路径规划师 — 联动保险与移民签证的家庭未来规划智能助手。

## 核心理念

不是简单地从产品库里搜产品，而是把保险与移民签证项目放进同一张"家庭未来规划地图"里。当客户提出子女教育、身份配置、家庭保障、跨境生活安排等需求时，输出**路径级答案**——先解决身份、同步补齐保障、再进入落地材料清单与顾问跟进节点。

## 安装

```bash
npm install -g @gloryfham/mcp-global-planner
```

## 使用

### 作为 Claude Code Skill

```bash
npx skills add gloryfham/agent-skills
```

### 作为独立 MCP Server

```bash
npx @gloryfham/mcp-global-planner
```

## 可用工具

### 保险产品查询

| 工具 | 参数 | 描述 |
|------|------|------|
| `listInsuranceProducts` | 无 | 获取所有保险产品列表 |
| `searchInsuranceProducts(keyword?, productType?, region?)` | 全部可选 | 搜索保险产品 |
| `getInsuranceProductDetail(productCode)` | productCode(必填) | 获取产品详情 |

### 签证/移民项目查询

| 工具 | 参数 | 描述 |
|------|------|------|
| `listVisaProjectTypes` | 无 | 获取所有项目类型分类 |
| `listAllVisaProjects` | 无 | 获取所有签证/移民项目列表 |
| `searchVisaProjects(keyword?, country?, projectType?, identityType?, minAmount?)` | 全部可选 | 搜索签证/移民项目 |
| `getVisaProjectDetail(projectCode)` | projectCode(必填) | 获取项目详情 |

### 核心：路径规划

| 工具 | 描述 |
|------|------|
| **`generateFamilyPathPlan`** | 根据家庭情况生成身份规划与保险保障的联动路径建议 |

`generateFamilyPathPlan` 参数：
- `primaryGoal` (必填) — 主要目标：`identity`(身份配置) | `insurance`(保障优先) | `education`(子女教育) | `retirement`(养老规划) | `comprehensive`(全面规划)
- `targetCountries` (可选) — 目标国家/地区列表
- `familyStructure` (可选) — 家庭结构描述
- `timeWindow` (可选) — 期望完成时间窗口
- `hasExistingVisa` (可选) — 是否已有海外身份
- `hasExistingInsurance` (可选) — 是否已有商业保险
- `budget` (可选) — 预算范围

## License

MIT
