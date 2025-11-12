# Thuật toán Support Vector Machine
* **Thuật toán Support Vector** Machine mục tiêu dùng để tìm ra được 1 đường phân cách tốt nhất để có thể phân chia các điểm dữ liệu trong không gian đa chiều
    * Thuật toán này có performance có hiệu suất rất cao với các bộ dữ liệu đa chiều và phân loại dữ liệu 


* Các điểm dữ liệu thuộc về các class mà gần với đường phân cách tối ưu nhất được gọi là support vector.

* Không phải lúc nào **"Support Vector Machine"** cũng tìm được đường phân cách tối ưu cho các điểm dữ liệu mà không có bất kỳ sai sót nào => Vì thế trong quá trình xây dựng thuật toán người ta có tạo 1 tham số **Hyperparameter là: C** (Ngưỡng chấp nhận có 1 vài số phân loại sai)

### KERNEL TRICK
* Có nhiều trường hợp chúng ta không phải lúc nào cũng có thể kẻ được 1 đường thẳng kẻ 1 đường tuyến tính để phân chia các điểm dữ liệu về 2 phía của đường thẳng
* Vậy nên có 1 phương pháp đó là Kernal trick đưa các điểm dữ liệu từ không gian 2 chiều thành không gian 3 chiều. Giúp dữ liệu có thể dễ dàng hơn phân chia được 1 cách tuyến tính (thông qua 1 mặt phẳng)

##### KERNAL TRICK là gì ?

## Multi-clas Support Vector Machine
* Multi-classs SVM là cách mở rộng để sử dụng được nhiều hơn SVM thông thường để giải quyết bàu toán có nhiều lớp

##### SO SÁNH HIỆU QUẢ GIỮA MULTI-CLASS SVM và SVM thông thường
* **Multi-class Support Vector Machine** là cách giải quyết khi có nhiều hơn **hai nhóm** cần phân loại (ví dụ: "SUV", "Sedan", "Pickup"). SVM thông thường chỉ xử lý được hai nhóm bằng cách tìm một mặt phẳng tối ưu duy nhất để phân chia 2 lớp. Còn Multil Class SVM xây dựng nhiều mặt phẳng thông qua các chiến lược chính là OvO và OvR 

##### Chiến lược OvO:
* Tạo ra mô hình SVM cho mỗi cặp lớn. Nếu có N lớp sẽ có **N*(N-1)/2** mô hình
 
