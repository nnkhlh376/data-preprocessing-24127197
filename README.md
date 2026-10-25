# Đồ án Tiền xử lý dữ liệu — 24127197

Đồ án môn Khai thác dữ liệu (HCMUS): cài đặt, so sánh và giải thích các kỹ thuật tiền xử lý
cho **dữ liệu bảng** (Home Credit Default Risk) và **dữ liệu văn bản** (IMDb Movie Reviews).

- Đề bài: <https://hcmus-cs-ta.github.io/lab-book/data-mining/projects/preprocessing/>
- Book: <https://nnkhlh376.github.io/data-preprocessing-24127197/>

## Dữ liệu

| Phần | Dataset | Nguồn | Đặt tại |
|---|---|---|---|
| Bảng | Home Credit — `application_train.csv`, `HomeCredit_columns_description.csv` | [Kaggle](https://www.kaggle.com/competitions/home-credit-default-risk/data) | `data/raw/home_credit/` |
| Văn bản | IMDb (25.000 train / 25.000 test) | [Hugging Face](https://huggingface.co/datasets/stanfordnlp/imdb) | tải bằng thư viện `datasets` |

Dữ liệu thô không được đưa lên GitHub. Danh sách ID chia tập nằm ở `data/splits/` để tái lập.

## Cấu trúc

```text
book/        notebook và báo cáo (tabular/, text/)
src/         hàm dùng chung
data/        raw/ (không commit), processed/, splits/
results/     bảng và hình từ thí nghiệm thật
```

## Chạy lại

```bash
python -m venv .venv
.venv\Scripts\activate          # Windows
pip install -r requirements.txt
jupyter lab
```

Mở notebook trong `book/` và chạy từ trên xuống. Notebook tự tìm thư mục gốc repo,
nên có thể mở từ bất kỳ thư mục con nào.

## Build book

Book dùng [Jupyter Book 2](https://jupyterbook.org) (cần Node.js ≥ 18), cấu hình tại `book/myst.yml`.

```bash
cd book
jupyter book start          # xem trước tại http://localhost:3000
jupyter book build --html   # xuất HTML vào book/_build/html
```

Mỗi lần push lên `main`, workflow `.github/workflows/deploy-book.yml` tự build và xuất bản lên
GitHub Pages. Book hiển thị output đã lưu trong notebook; notebook không được chạy lại trên CI.
