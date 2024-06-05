# What we do

1. Generate for me three datasets. Each dataset has 1 training set with 10 data points and 1 test set with 10 data points. Data points (x,y) have input value x generated randomly in the range [0,1], and target value y = f(x)=sin(1+x^2)+ε with ε is the standard deviation and follows the normal distribution N(0,σ=0.03).

2. For each data set, use the training set to train 9 polynomial regression models with degrees from 1-9, plot 9 polynomial in one picture for each dataset. Then, calculate E_in (on the training set) and E_out (on the test set) for each trained model, and create table as shown on degree with its E_in and E_out. E_in  and E_out write with 5 decimal after dotted. 



Với mỗi bộ dữ liệu, ta sử dụng tập train để huấn luyện 9 mô hình polynomial regression có bậc (degree) từ 1-9 như trong trang 65 của slides. Sau đó, hãy tính E_in (trên tập train) và E_out (trên tập test) cho từng mô hình đã huấn luyện được, và tạo bảng kết quả như trong trang 66 của slides.

Làm tương tự như trên cho cả 03 bộ dữ liệu D1, D2, D3 để có được hình minh họa như trong trang 68 của slides. Cần ghép được 9 hình nhỏ trong cùng 1 hình lớn.
Các bạn có nhận xét thế nào về bias và variance của các mô hình?
03 bộ dữ liệu trên tập train chỉ có kích thước là 10. Chúng ta hãy thử kích thước tập train và test (100, 1000 điểm dữ liệu), và lặp lại các thực nghiệm từ 1-4 như trên. 
Sử dụng kết quả thực nghiệm và trực quan hóa, để trả lời thêm 2 câu hỏi sau:
Tăng kích thước tập train có thể giảm bias của mô hình hay không?
Tăng kích thước tập train có thể giảm variance của mô hình hay không?
LƯU Ý: Trong file ipynb bài nộp, cần có 1 đoạn code như sau nằm ở đầu file sau khi import các thư viện numpy và trước khi phát sinh dữ liệu với MSHV là dãy các chữ số trong mã số học viên cao học của mỗi bạn.

    seed = MSHV
    np.random.seed(seed)
    random.seed(seed)