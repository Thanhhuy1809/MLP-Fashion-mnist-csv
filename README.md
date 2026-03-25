MLP Fashion-MNIST (CSV)
Phân loại Fashion-MNIST từ file CSV (cột label + 784 pixel ảnh 28×28) bằng MLP (Multi-Layer Perceptron) với TensorFlow/Keras. Notebook chính: MLP.ipynb

Dataset
Train: fashion-mnist_train.csv
Test: fashion-mnist_test.csv
Ghi chú: file train lớn (>100MB) nên repo dùng Git LFS để lưu/pull dữ liệu.

Yêu cầu môi trường
Python 3.9+ (khuyến nghị)
Thư viện: numpy, matplotlib, tensorflow (và pandas là tuỳ chọn)
Cài nhanh:
           pip install numpy matplotlib tensorflow pandas
Cách chạy
Clone repo:
git clone https://github.com/Thanhhuy1809/MLP-Fashion-mnist-csv.git
cd MLP-Fashion-mnist-csv
Pull dữ liệu (Git LFS):
git lfs install
git lfs pull

Mở MLP.ipynb và Run All cells (VS Code / Jupyter).
Nội dung notebook
Đọc CSV, tách X/y, chuẩn hoá pixel về [0..1]
Tách validation từ train để theo dõi overfitting
Xây dựng MLP (Dense + ReLU + Dropout, output Softmax 10 lớp)
Huấn luyện, đánh giá train/val/test
Trực quan hoá một số mẫu ảnh và dự đoán
Ghi chú
Nếu clone xong mà thiếu dữ liệu, hãy chạy lại git lfs pull.
Có thể chỉnh siêu tham số (epochs, batch size, learning rate, hidden units, dropout) trực tiếp trong notebook.
