# 白皮書 (Whitepaper)

## 背景與動機
戰役戰術知識檢索需要快速、準確且可解釋的系統。

## 系統設計理念
- 模組化設計：ETL → Embedding → Vector DB → Retrieval → Reranker
- 高效檢索：Hybrid Search + Parent-Document Retrieval
- 可解釋性：提供檢索來源透明度

## 技術選型理由
- **BGE-M3**：多語言支援，適合軍事文本
- **pgvector**：Postgres 原生支援，易於維護
- **Hybrid Search**：結合語義與關鍵字檢索
- **Reranker**：提升答案排序準確度

## 使用情境
- 戰術案例查詢
- 軍事知識教育
- 戰役資料分析

## 未來改進方向
- 引入知識圖譜
- 增加多模態檢索 (文字 + 圖像)

## 理論深度
戰役戰術知識轉換為向量表徵的挑戰：戰術語境依賴、專有名詞多。

## 創新性
- 解決 hallucination：透過 Reranker + 知識圖譜驗證。
- 冷啟動問題：建立軍事專有名詞詞典（例如 NATO 縮寫、武器代號）。
