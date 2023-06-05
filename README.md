# ML_Projects
> Đây là dự án cuối kỳ đối với môn học "Học máy". Tên đề tài được chọn là "Ứng dụng học máy trong việc nhận diện khuôn mặt".
___
## Thành viên nhóm:
Khuất Đăng Sơn 20002159 (<b>C</b>) ([github_link](https://github.com/Thefuckingdead))

Nguyễn Thị Thanh 20002164 ([github_link](https://github.com/NguyenThiThanhNguSi))

Trần Thiên Cường 20002109 ([github_link](https://github.com/TranThienCuong))

Luyện Thị Quyên 20002158 ([github_link](https://github.com/LuyenQuyen))

Nguyễn Trọng Trưởng 20002172 ([github_link](https://github.com/NguyenTrongTruong))
___
## Cấu trúc các thư mục
Trong cả thư mục lớn này bao gồm thư mục nhỏ, mỗi thư mục nhỏ lại tương đương việc giải quyết 1 bài toán trong việc phân loại hình ảnh. Các bài toán được chọn bao gồm 3 bài toán: **Nhận diện gương mặt sinh viên**, **Nhận diện cảm xúc**, **Nhận diện người nổi tiếng (Format theo kiểu What you look like?)**. Trong đó:
- <b>Emotion_Face_Classifier</b>: Đây là thư mục chứa dự án nhận diện cảm xúc người dùng (**Chú ý**: Độ chính xác của mô hình này khá thấp (~ 45%)) (dataset gốc: [click here](https://drive.google.com/drive/folders/1JShtGEyzQSp3Nq6vlx_sn-pDahCrK81e?usp=share_link))
- <b>Movie_Star_Classification</b>: Đây là thư mục chứa dự án nhận diện người nổi tiếng (**độ chính xác: ~ 80%**)
- <b>Student_Recognize_Project</b>: Đây là thư mục chứa dự án nhận diện sinh viên (**độ chính xác: ~ 95%**) (có thể thay đổi model, đọc kỹ phần code trong util.py)
___
## Công nghệ được sử dụng
- Ngôn ngữ sử dụng:
<p>
  <a>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f8/Python_logo_and_wordmark.svg/1280px-Python_logo_and_wordmark.svg.png" height="30" width="120">
  </a>
  
   <a>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/61/HTML5_logo_and_wordmark.svg/2048px-HTML5_logo_and_wordmark.svg.png" height="30" width="30">
  </a>
  
  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d5/CSS3_logo_and_wordmark.svg/1200px-CSS3_logo_and_wordmark.svg.png" height="30" width="20">
  </a> 
  
  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d4/Javascript-shield.svg/1200px-Javascript-shield.svg.png" height="30" width="20">
  </a>
</p>
- Xây dựng mô hình học máy (Thư viện sử dụng): 
<p>
  <a>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/84/Matplotlib_icon.svg/1200px-Matplotlib_icon.svg.png" height="30" width="30">
  </a>

  <a>
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/32/OpenCV_Logo_with_text_svg_version.svg/831px-OpenCV_Logo_with_text_svg_version.svg.png" height="30" width="30">
  </a>

  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/2560px-NumPy_logo_2020.svg.png" height="30" width="80">
  </a>
  
   <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ed/Pandas_logo.svg/2560px-Pandas_logo.svg.png" height="30" width="80">
  </a>
  
  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/05/Scikit_learn_logo_small.svg/1200px-Scikit_learn_logo_small.svg.png" height="30" width="50">
  </a>
</p>

- Các ide được sử dụng:
<p>
  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Visual_Studio_Code_1.35_icon.svg/2048px-Visual_Studio_Code_1.35_icon.svg.png" height="30" width="30">
  </a>
  
  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Google_Colaboratory_SVG_Logo.svg/2560px-Google_Colaboratory_SVG_Logo.svg.png" height="30" width="50">
  </a>
</p>

- Backend (Thư viện Flask):
<p>
  <a>
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3c/Flask_logo.svg/1280px-Flask_logo.svg.png" height="30" width="100">
  </a>
</p>

___

## Lưu đồ

1. Lưu đồ tổng quan
![General_Model](https://github.com/Thefuckingdead/ML_Projects/assets/95278548/d1d84ae6-7f09-4b33-938b-d647654024f7)

2. Lưu đồ xây dựng mô hình học máy
![Machine Learning Process](https://github.com/Thefuckingdead/ML_Projects/assets/95278548/7051860b-61cd-4bb6-a0b4-70f6ffe8a3c9)
___
## Nhận diện khuôn mặt sinh viên
### Cách thức cài đặt
- Truy cập vào thư mục "Student_Recognize_Project". Sau khi đã vào được thư mục trên tạo 1 môi trường ảo python với câu lệnh:
```python
virtualenv your_env_name
```
- Trong đó your_env_name là tên môi trường mà bạn muốn đặt. Sau khi cài xong môi trường ảo kích hoạt môi trường đó thông qua câu lệnh
```python
.\your_env_name\Script\activate
```
- Sau khi thực hiện câu lệnh trên thì cài đặt các gói phần mềm cần sử dụng thông qua câu lệnh
```python
pip install -r requirements.txt
```
- Chạy xong câu lệnh trên truy cập vào folder "Server" và chạy câu lệnh
```python
python server.py
```
Chạy xong câu lệnh trên là ta có thể chạy được chương trình của chúng ta rồi :)
### Chạy và hiện kết quả
- Truy cập vào thư mục "UI" và mở html lên. Giao diện nhận được sẽ như sau
![image](https://github.com/Thefuckingdead/ML_Projects/assets/95278548/79def14e-3bb7-446f-8e76-95f1fe5b0db2)
- Sau khi kéo ảnh lên và ấn nút "classify" sẽ nhận được kết quả
![image](https://github.com/Thefuckingdead/ML_Projects/assets/95278548/00a3bba8-24ae-4411-b57e-9891b1af82b6)
___
## Nhận diện người nổi tiếng (Bạn giống ai ?)
### Cách thức cài đặt
- Tương tự như trên thay vì truy cập vào thư mục "Student_Recognize_Project" thì truy cập vào thư mục "Movie_Star_Classification"
- Cấu trúc các thư mục khác tương tự.
### Chạy và hiện kết quả
- Truy cập vào thư mục "UI" và mở html lên. Giao diện nhận được sẽ như sau
![image](https://github.com/Thefuckingdead/ML_Projects/assets/95278548/cd6c9763-f614-42ed-8d35-dd047605c5ce)
- Sau khi kéo ảnh lên và ấn nút "classify" sẽ nhận được kết quả
![image](https://github.com/Thefuckingdead/ML_Projects/assets/95278548/cad72ce0-5050-4cc2-b989-2713fac75158)
___
## Nhận diện cảm xúc
### Cách thức cài đặt
- Tương tự như trên thay vì truy cập vào thư mục "Student_Recognize_Project" thì truy cập vào thư mục "Emotion_Face_Classification"
- Cấu trúc các thư mục khác tương tự.
### Chạy và hiện kết quả
- Truy cập vào thư mục "UI" và mở html lên. Giao diện nhận được sẽ như sau
![image](https://github.com/Thefuckingdead/ML_Projects/assets/95278548/e6e70aef-5933-4616-9387-0f75dbe3590c)
- Sau khi kéo ảnh lên và ấn nút "classify" sẽ nhận được kết quả
![image](https://github.com/Thefuckingdead/ML_Projects/assets/95278548/6cf120a9-d0e8-46f7-97a8-5a14138e83b4)
___
## Kết luận
Qua bài tập lớn trên nhóm chúng em đã làm được ứng dụng được việc sử dụng các mô hình học máy để giải quyết các bài toán về nhận diện gương mặt như **Nhận diện gương mặt sinh viên, Nhận diện cảm xúc, Nhận diện người nổi tiếng**.
### Khó khăn
Tuy nhiên nhóm chúng em đã làm được những bài toán trên nhưng mới chỉ 1 phần nào đó. Vẫn còn những thiếu sót như việc chọn mô hình chưa được tối ưu, đối với thời buổi hiện tại thì phương pháp tối ưu nhất vẫn là ứng dụng việc học sâu để giải quyết các vấn đề nhận diện khuôn mặt với CNN. Ngoài ra web app mà nhóm tạo được vẫn chỉ chạy trên local chưa đẩy lên cloud khá là sơ sài.
### Phương hướng phát triển tương lai
Thay vì chỉ sử dụng mỗi mô hình học máy, nhóm sẽ phát triển ứng dụng mô hình học sâu và sử dụng các mô hình như CNN để giải quyết bài toán 1 cách hiệu quả hơn. Ngoải ra nhóm cũng sẽ cố gắng phát triển thêm thay vì một web app sơ sài chạy riêng biệt từng dự án như vậy thì sẽ tích hợp thành 1 web app hoàn chỉnh có thể điều hướng sử dụng tất cả mô hình trên cũng như việc phát triển tích hợp mô hình huấn luyện được vào mobile app cũng như pc app. Tất nhiên điều kiện tiên quyết là mô hình phải đáp ứng được các nhu cầu khắt khe cũng như độ chính xác phải cao thì mới đưa đến tay người dùng thực tế.
___
## Tài liệu tham khảo
1. codebasics, machine learning | Sport celebrity image classification, URL: https://www.youtube.com/playlist?list=PLeo1K3hjS3uvaRHZLl-jLovIjBP14QTXc
2. wikipedia, wavelet transform, URL: https://en.wikipedia.org/wiki/Wavelet_transform
3. Global Software Support, Computer Vision - Haar-Features, URL: https://www.youtube.com/watch?v=F5rysk51txQ
4. codebasics, Machine Learning Tutorial Python - 16: Hyper parameter Tuning (GridSearchCV), URL: https://www.youtube.com/watch?v=HdlDYng8g9s&list=PLeo1K3hjS3uvCeTYTeyfe0-rN5r8zn9rw&index=17
5. Viblo.asia, KNN (K-Nearest Neighbors), URL: https://viblo.asia/p/knn-k-nearest-neighbors-1-djeZ14ejKWz 
