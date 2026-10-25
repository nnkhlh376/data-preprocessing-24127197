# Đồ án Tiền xử lý dữ liệu

**Sinh viên:** *(họ tên)* — **MSSV:** 24127197
**Môn:** Khai thác dữ liệu — HCMUS
**Đề bài:** <https://hcmus-cs-ta.github.io/lab-book/data-mining/projects/preprocessing/>

## Mục tiêu

> *(Viết 3–5 câu: đồ án làm gì, vì sao tiền xử lý quan trọng, cách tiếp cận so sánh thí nghiệm rồi chọn pipeline.)*

## Dữ liệu

| Phần | Dataset | Bài toán | Kích thước |
|---|---|---|---|
| (a) Bảng | Home Credit Default Risk — `application_train.csv` | Dự đoán khó khăn thanh toán (TARGET 0/1) | 307.511 dòng × 122 cột |
| (b) Văn bản | IMDb Movie Reviews | Phân loại cảm xúc (0 tiêu cực / 1 tích cực) | 25.000 train + 25.000 test |

## Nguyên tắc thí nghiệm

> *(Tóm tắt: chia train/test trước, mọi bước fit trong fold, các phương pháp là nhánh song song cùng điều kiện, test chỉ đánh giá một lần.)*

## Nội dung

**Phần (a) — Dữ liệu bảng**
1. Tổng quan dữ liệu và baseline
2. EDA chuyên sâu
3. Xử lý giá trị thiếu
4. Phát hiện ngoại lai
5. Chuẩn hóa và mã hóa
6. Lựa chọn và giảm chiều đặc trưng
7. [Nâng cao] Mất cân bằng lớp
8. Pipeline cuối

**Phần (b) — Văn bản**
1. Tổng quan và Text EDA
2. Làm sạch và tokenization
3. Stop words, stemming, lemmatization
4. Vector hóa
5. [Nâng cao] Sentence Transformer
6. Pipeline cuối

**Báo cáo tổng hợp:** so sánh, thảo luận và hạn chế.
