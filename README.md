# ds_dandangi_raj-PrimeTradeAI-

---

this projects aimed on the  objective is to explore the relationship between trader performance and market 
sentiment, uncover hidden patterns, and deliver insights that can drive smarter trading 
strategies.
provided assests : 1.Historical Trader Data from Hyperliquid  , 2. Bitcoin Market Sentiment Dataset

---

step 1 : work flowchart & steps performed on dataset 1. Historical Trader Data from Hyperliquid

```mermaid
graph TD
    A[Start] --> B{Load Data}
    B --> C[Authenticate and Load Historical Data]
    C --> D[Initial Data Inspection<br>shape, info, dtypes]
    D --> E{EDA}
    E --> F["Check for Missing Values<br>isnull().sum(), missingno.matrix()"]
    E --> G["Find Unique Values<br>nunique(), unique()"]
    G --> H{Data Cleaning}
    H --> I[Remove Duplicates]
    H --> J[Remove Special Characters<br>from Coin column]
    H --> K[Convert Data Types<br>float, int, bool, category, datetime]
    K --> L{Fix Errors/Inconsistencies}
    L --> M[Convert Trade ID & Timestamp to Numeric]
    L --> N[Handle Duplicate Trade IDs<br>Create Fixed_Trade_ID]
    L --> O[Validate Fee Discrepancy]
    L --> P[Convert Timestamp to Datetime<br>create timestampfix]
    L --> Q[Handle NaN in Discrepancy_Percent]
    Q --> R{Explore Data Characteristics<br>Univariate Analysis}
    R --> S[Analyze Numerical Columns<br>stats, skewness, transformations]
    R --> T[Analyze Categorical Columns<br>value counts, frequency plots]
    T --> U{Multivariate Analysis}
    U --> V[Correlation Matrix<br>Numerical Columns]
    U --> W[Scatter Plots<br>Key Numerical Relationships]
    W --> X[Visualize Actual vs. Expected Fee]
    X --> Y[End]
```
