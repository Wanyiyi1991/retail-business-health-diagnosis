# 🏪 零售业务健康度诊断分析

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-brightgreen)](https://pandas.pydata.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> 对公司交易数据进行全面诊断，找出利润黑洞并给出可执行的业务建议。
> 数据集来源：Sample_Superstore.csv from [Kaggle](https://www.kaggle.com/datasets/naveenkumar20bps1137/sample-superstore)

## 📊 项目概览

对 **9,994 笔订单**进行从整体到细节的多维度分析，并构建 **RFM 客户价值模型**，将客户分为 4 个层级，输出精准的留存与营销策略。

## ❓ 回答的核心问题

| 序号 | 业务问题 | 分析维度 |
|------|----------|----------|
| 1 | 公司整体增长趋势如何？有无季节性？ | 月度销售与利润趋势 |
| 2 | 哪个品类在赚钱，哪个在亏钱？ | 品类/子品类利润分析 |
| 3 | 亏损集中在哪里？ | 地区利润分布 |
| 4 | 亏损的根本原因是什么？ | 折扣与利润的关系 |
| 5 | 高价值客户长什么样？ | RFM 客户分层 |

## 🔍 核心发现

1. **Furniture品类是利润黑洞**：Tables子品类累计亏损$17,000+，根源是高达30%+的折扣
2. **Central地区问题突出**：尤其是德克萨斯州和伊利诺伊州，贡献了最大的负利润
3. **9月旺季利润反常下降**：促销期间高折扣低利润产品占比过高
4. **18.5%的Champion客户贡献了62%的收入**：仅158人撑起大半江山
5. **35%的客户处于流失风险中**：At Risk群体需立即触达

## 🛠 技术栈

- **数据清洗**: Pandas, NumPy
- **可视化**: Matplotlib, Seaborn, Plotly
- **分析方法**: EDA(探索性分析), RFM模型, 四象限分析, 帕累托分析

## 📁 项目结构

├── notebooks/superstore_analysis.ipynb  
├── images/                            
├── report/analysis_report.md           
└── data/Sample_Superstore.csv        

## 🚀 快速复现

\```bash
# 1. 克隆仓库
git clone https://github.com/Wanyiyi1991/retail-business-health-diagnosis.git
cd retail-business-health-diagnosis

# 2. 安装依赖
pip install -r requirements.txt

# 3. 启动 Jupyter
jupyter notebook notebooks/superstore_analysis.ipynb
\```

## 📈 关键可视化

### 四象限客户价值分布
![RFM四象限]

### 利润黑洞：子品类分析
![子品类利润]

## 📝 业务建议（摘要）

1. **立即止血**：对Furniture品类的Tables、Bookcases折扣设上限(≤20%)
2. **旺季优化**：9月促销捆绑高利润Technology配件
3. **客户挽回**：对右上角“流失高危”大客户发送专属回归礼包
4. **核心维护**：Champion客户专享年度优惠和VIP客服通道

## 👤 关于我
一个数据分析探索者、爱好者！
QQ:783899056
E-mail:wanyiyi1991@gmail.com
---
⭐ 如果这个项目对你有帮助，欢迎给个Star！
