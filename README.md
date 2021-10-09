# Vietnamese-News-Classification
Giải quyết bài toán Text Classification bằng nhiều phương pháp khác nhau và so sánh

Dữ liệu là các bản tin tiếng Việt từ 27 topics khác nhau. Data source: https://github.com/duyvuleo/VNTC

### 1. Quá trình tiền xử lý
- Xóa HTML code nếu có
- Chuẩn hóa bảng mã Unicode
- Chuẩn hóa kiểu gõ dấu tiếng việt
- Thực hiện tách từ tiếng Việt
- Đưa về dạng việt thường
- Xóa các ký tự đặc biệt
- Loại bỏ stopwords
### 2. Quá trình huấn luyện model
Các phương pháp được sử dụng:
- Nhóm phương pháp Machine Learning
  + Bag-of-Words + TF-IDF + Machine Learning Classifier (Best: Logistic Regression 90.11%)
  + Doc2Vec + Machine Learning Classifier (Best: Logistic Regression 80.27%)
  + Doc2Vec + KNN (Best: 80.67%)
  + BERT + Machine Learning Classifier (Best: SVM 88.59%)
  + Fine-tune BERT (Best: 92.36%)

### 3. Kết luận
Phương pháp cho kết quả tốt nhất và cũng là phức tạp nhất cho bài toán Text Classifier là Fine-tune lại mô hình BERT.

