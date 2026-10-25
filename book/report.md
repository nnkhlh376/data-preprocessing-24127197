# Báo cáo tổng hợp

> Viết sau khi đã có kết quả thật từ các notebook. Mỗi kết luận dẫn về notebook và bảng kết quả tương ứng.

## 1. Tóm tắt

> *(Kết quả chính của hai phần trong 5–8 câu.)*

## 2. Phần (a) — Dữ liệu bảng

| Bước | Các phương án đã thử | Phương án chọn | Lý do (dẫn số liệu) |
|---|---|---|---|
| Giá trị thiếu | mean, median, mode, KNN (k=3,5,10), MICE | | |
| Ngoại lai | IQR, Z-score, Isolation Forest, LOF, DBSCAN | | |
| Chuẩn hóa | Min-Max, Z-score, Robust, Quantile | | |
| Mã hóa | One-Hot, Ordinal, Target, Binary, Frequency | | |
| Chọn đặc trưng | ANOVA, Chi-square, MI, RF, GB, RFE-CV, PCA | | |
| Mất cân bằng | SMOTE, ADASYN, Under-sampling | | |

> *(Kết quả test cuối, so sánh với baseline, thảo luận.)*

## 3. Phần (b) — Văn bản

| Bước | Các phương án đã thử | Phương án chọn | Lý do (dẫn số liệu) |
|---|---|---|---|
| Làm sạch | | | |
| Tokenization | word, sentence, character, BPE | | |
| Stop words | giữ, bỏ, bỏ trừ phủ định | | |
| Dạng từ | Porter, Snowball, WordNet | | |
| Vector hóa | BoW, TF-IDF n=1,2,3, Word2Vec, Sentence Transformer | | |

> *(Kết quả test cuối, so sánh với baseline, thảo luận.)*

## 4. Thảo luận chung

> *(Những gì rút ra về tiền xử lý: khi nào kỹ thuật phức tạp có lợi, đánh đổi chi phí, leakage.)*

## 5. Hạn chế và hướng phát triển

## 6. Tài liệu tham khảo
