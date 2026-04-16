# 荣耀全球路径规划师

Glory Global Path Planner MCP Server — 联动保险与移民签证的家庭未来规划智能助手。

## 核心理念

不是简单地从产品库里搜产品，而是把保险与移民签证项目放进同一张"家庭未来规划地图"里。当客户提出子女教育、身份配置、家庭保障、跨境生活安排等需求时，输出**路径级答案**——先解决身份、同步补齐保障、再进入落地材料清单与顾问跟进节点。

## 安装

```bash
npm install -g gloryfham-mcp-global-planner
```

## 使用

### 作为 Claude Code Skill

```bash
npx skills add sergio-wen/mcp-global-planner
```

### 作为独立 MCP Server

```bash
npx gloryfham-mcp-global-planner
```

## 可用工具

| 工具 | 描述 |
|------|------|
| `listInsuranceProducts` | 获取所有保险产品列表 |
| `searchInsuranceProducts` | 搜索保险产品 |
| `getInsuranceProductDetail` | 获取保险产品详情 |
| `listVisaProjectTypes` | 获取签证项目类型分类 |
| `listAllVisaProjects` | 获取所有签证/移民项目列表 |
| `searchVisaProjects` | 搜索签证/移民项目 |
| `getVisaProjectDetail` | 获取签证项目详情 |
| **`generateFamilyPathPlan`** | **核心：生成家庭身份+保障联动路径建议** |

## License

MIT
