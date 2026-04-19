# 規格說明書 (Specs)

## Chunking Strategy
- 固定長度：512 tokens
- 語義切分：依照戰術章節

## 性能指標
- Latency ≤ 200ms
- Top-5 準確度 ≥ 85%

## 評估機制
- 使用 RAGAS / TruLens 測試忠實度、相關性、完整度
