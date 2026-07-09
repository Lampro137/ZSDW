# "置身钉内"小红书舆情分析可视化报告

基于小红书平台 651 篇笔记、9,026 条评论的实证数据，对钉钉换帅"置身钉内"舆情传播机制与公众情绪特征的系统分析可视化报告。

## 在线预览

部署到 GitHub Pages 后，访问 `https://<你的用户名>.github.io/<仓库名>/` 即可在线查看报告。

## 部署到 GitHub Pages

### 方式一：新建仓库部署（推荐）

1. 在 GitHub 上新建一个仓库（如 `sentiment-report`）
2. 将 `github-deploy` 目录下的所有文件推送到该仓库：

```bash
cd github-deploy
git init
git add .
git commit -m "Initial commit: sentiment analysis report"
git branch -M main
git remote add origin https://github.com/<你的用户名>/sentiment-report.git
git push -u origin main
```

3. 进入仓库 Settings → Pages → Source 选择 `main` 分支
4. 等待约 1 分钟，访问 `https://<你的用户名>.github.io/sentiment-report/`

### 方式二：已有仓库中添加

将 `index.html` 和 `.nojekyll` 放入已有仓库的根目录或 `docs/` 子目录，然后在 Settings → Pages 中选择对应分支和目录即可。

## 项目结构

```
github-deploy/
├── index.html      # 主页面（自包含 HTML，ECharts 通过 CDN 加载）
├── .nojekyll       # 防止 GitHub Pages 用 Jekyll 处理
└── README.md       # 本说明文件
```

## 技术栈

- **前端**：纯 HTML + CSS + JavaScript，无构建依赖
- **图表库**：ECharts 5.5.0（CDN 加载）
- **字体**：系统字体栈（PingFang SC / Microsoft YaHei 等）

## 报告内容

| 章节 | 内容 |
|---|---|
| 01 研究背景 | 事件溯源与 4 个核心研究问题 |
| 02 数据与方法 | 数据规模、处理流程、工具栈 |
| 03 核心人物与事件 | 人物覆盖率、事件覆盖率、高频词 |
| 04 话题聚类 | 9 大主题分布、关键词讨论侧重雷达图 |
| 05 社交网络分析 | 网络指标、Top5 传播节点、用户角色、漏斗传播路径 |
| 06 情感分析 | 笔记/评论情感分布与对比 |
| 07 传播机制 | KOL 驱动、跨社区桥梁、评论区极化、竞品叙事 |
| 08 风险评估 | 5 大风险维度卡片 |
| 09 政策建议 | 6 条系统性应对路径 |
| 10 结论 | 4 大研究问题的总结回答 |

## 特性

- 响应式设计，适配桌面与移动端
- 10 个交互式 ECharts 图表（悬停可查看详细数据）
- 无需服务器，纯静态文件，直接浏览器打开即可运行
- 中文排版优化

## 本地预览

直接双击 `index.html` 用浏览器打开即可查看完整报告，无需任何本地服务器。
