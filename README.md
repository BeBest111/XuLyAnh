# Xử Lý Ảnh - Nhận Diện Khuôn Mặt và Mắt

## Mô tả

Dự án này sử dụng các thư viện Python và OpenCV để thực hiện nhận dạng khuôn mặt và mắt trong ảnh hoặc video, dựa trên bộ phân loại Haar Cascade.

## Tính năng

* Phát hiện khuôn mặt từ hình ảnh/video
* Phát hiện mắt trên khuôn mặt đã nhận diện
* Áp dụng các phép biến đổi hình ảnh như: làm mờ, thay đổi độ sáng, xoay ảnh,...
* Giao diện trực quan qua Jupyter Notebook (`ImageTransformations.ipynb`)

## Công nghệ sử dụng

* Python 3.x
* OpenCV
* NumPy
* Jupyter Notebook

## Tệp quan trọng

* `ImageTransformations.ipynb`: Notebook chính chứa mã nguồn xử lý ảnh
* `haarcascade_frontalface_default.xml`: Bộ phân loại Haar để nhận diện khuôn mặt
* `haarcascade_eye.xml`: Bộ phân loại Haar để nhận diện mắt

## Cách sử dụng

1. Cài đặt các thư viện cần thiết:

   ```bash
   pip install opencv-python numpy
   ```
2. Mở tệp notebook:

   ```bash
   jupyter notebook ImageTransformations.ipynb
   ```
3. Thực thi các ô trong notebook để xem kết quả.

## Ghi chú

* Các tệp `.xml` cần được giữ đúng đường dẫn khi nạp vào trong code OpenCV, ví dụ:

  ```python
  face_cascade = cv2.CascadeClassifier('haarcascade_frontalface_default.xml')
  eye_cascade = cv2.CascadeClassifier('haarcascade_eye.xml')
  ```

## Bản quyền

Các mô hình Haar Cascade được cung cấp bởi OpenCV theo giấy phép của Intel. Vui lòng xem chi tiết trong các tệp `.xml`.
