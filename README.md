# 社群媒體使用對學生影響分析

本專案分析社群媒體使用時間與學生身心健康之間的關係，包括心理健康、睡眠品質及成癮程度。

## 📊 資料集
**來源** kaggle: https://www.kaggle.com/datasets/adilshamim8/social-media-addiction-vs-relationships 

- 資料集包含學生的社群媒體使用模式及各項健康/行為指標：

| 欄位 | 說明 |
|------|------|
| `Student_ID` | 學生編號 |
| `Age` | 年齡 |
| `Gender` | 性別 |
| `Academic_Level` | 教育程度（高中 / 大學 / 研究所） |
| `Country` | 國家 |
| `Avg_Daily_Usage_Hours` | 每日平均使用社群媒體時數 |
| `Most_Used_Platform` | 最常使用的社群平台 |
| `Affects_Academic_Performance` | 是否影響學業表現（Yes/No） |
| `Sleep_Hours_Per_Night` | 每晚平均睡眠時數 |
| `Mental_Health_Score` | 心理健康分數（1-10 分） |
| `Relationship_Status` | 感情狀態 |
| `Conflicts_Over_Social_Media` | 因社群媒體產生的衝突次數 |
| `Addicted_Score` | 社群媒體成癮分數（1-10 分） |

## 🔍 主要發現

### 皮爾森相關係數分析（Pearson's r）

| 比較項目 | 相關係數 |
|----------|----------|
| 每日使用時數 vs. 成癮分數 | **+0.8320**（強正相關） |
| 每日使用時數 vs. 心理健康分數 | **-0.8011**（強負相關） |
| 每日使用時數 vs. 睡眠時數 | **-0.7906**（強負相關） |

### 研究結論

1. **成癮程度**：社群媒體使用時間越長，成癮分數越高
2. **心理健康**：使用時間增加與心理健康分數下降有顯著關聯
3. **睡眠品質**：花越多時間在社群媒體上，睡眠時數越少

## 📈 視覺化圖表

本 Notebook 包含：
- 使用時數分類分佈分析
- 各使用類別的趨勢折線圖
- 關鍵指標之間的相關性分析

## 🛠️ 環境需求

```
pandas
matplotlib
seaborn
scipy
numpy
```

## 🚀 使用方式

1. Clone 此專案
2. 安裝所需套件：
   ```bash
   pip install -r requirements.txt
   ```
3. 使用 Jupyter Notebook 或 JupyterLab 開啟 `g06.ipynb`

## 📁 專案結構

```
.
├── README.md           # 專案說明文件
├── g06.ipynb           # 主要分析 Notebook
├── requirements.txt    # Python 套件依賴
└── .gitignore          # Git 忽略設定
```

