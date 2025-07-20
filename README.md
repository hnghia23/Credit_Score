# HMEQ Loan Default Analysis

Phân tích dữ liệu khoản vay vốn chủ sở hữu nhà (Home Equity Loan) sử dụng bộ dữ liệu HMEQ. Dự án tập trung vào việc khám phá, xử lý và phân tích các yếu tố ảnh hưởng đến khả năng vỡ nợ của người vay, hỗ trợ trong việc đánh giá rủi ro tín dụng.

## Mục tiêu:
- Hiểu rõ các yếu tố ảnh hưởng đến rủi ro tín dụng.
- Hỗ trợ mô hình hóa dự đoán vỡ nợ trong tương lai.
- Làm nền tảng cho các hệ thống đánh giá tín dụng.

## 📊 Giới thiệu bộ dữ liệu

Bộ dữ liệu HMEQ gồm thông tin của **5.960 khoản vay**, với biến mục tiêu là `BAD` thể hiện việc người vay có vỡ nợ (1) hay không (0).
Dữ liệu được thu thập từ Kaggle: https://www.kaggle.com/datasets/ajay1735/hmeq-data

### Các trường dữ liệu chính:

| Trường      | Mô tả                                                             |
|-------------|-------------------------------------------------------------------|
| **BAD**     | 1 = vỡ nợ, 0 = không vỡ nợ                                        |
| **LOAN**    | Số tiền yêu cầu vay                                               |
| **MORTDUE** | Số tiền nợ còn lại trên thế chấp hiện tại                         |
| **VALUE**   | Giá trị tài sản hiện tại                                          |
| **REASON**  | Lý do vay: `DebtCon` (hợp nhất nợ), `HomeImp` (sửa sang nhà cửa)  |
| **JOB**     | Loại công việc                                                    |
| **YOJ**     | Số năm làm công việc hiện tại                                     |
| **DEROG**   | Số lần báo cáo vỡ nợ nghiêm trọng                                 |
| **DELINQ**  | Số hạn mức tín dụng quá hạn                                       |
| **CLAGE**   | Tuổi của hạn mức tín dụng lâu nhất (tháng)                        |
| **NINQ**    | Số yêu cầu tín dụng gần đây                                       |
| **CLNO**    | Tổng số hạn mức tín dụng                                          |
| **DEBTINC** | Tỷ lệ nợ/thu nhập                                                 |

## 📁 Nội dung

- `main.ipynb`: Notebook chính chứa toàn bộ quy trình phân tích.
- `description.txt`: Mô tả chi tiết về các trường trong bộ dữ liệu (tiếng Việt và tiếng Anh).

## 🔍 Các bước thực hiện

1. **Khám phá dữ liệu**: kiểm tra phân phối, số liệu thống kê, missing values.
2. **Xử lý dữ liệu**: điền thiếu, mã hóa biến phân loại, xử lý outlier.
3. **Phân tích**: mối liên hệ giữa các biến độc lập với khả năng vỡ nợ (`BAD`).
4. **Trực quan hóa**: sử dụng biểu đồ để minh họa đặc điểm dữ liệu và phát hiện xu hướng.

## ⚙️ Yêu cầu

- Python 3.x
- Jupyter Notebook
- Thư viện: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

