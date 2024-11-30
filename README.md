# Real-time Gender and Age Prediction from Webcam

## Mô tả dự án
Dự án này sử dụng mô hình học sâu để nhận diện giới tính và tuổi của người trong ảnh được chụp từ webcam trong thời gian thực. Mô hình sẽ phân tích ảnh từ webcam, dự đoán giới tính (Nam/Nữ) và độ tuổi ước tính, sau đó hiển thị kết quả dự đoán trực tiếp.

## Các yêu cầu
Để chạy ứng dụng này, bạn cần cài đặt các thư viện và công cụ sau:

1. **Python 3.6+**
2. **Các thư viện Python**:
   - `opencv-python`
   - `keras`
   - `numpy`
   - `matplotlib`

## Cài đặt

### Cài đặt các thư viện yêu cầu
Trước tiên, cài đặt các thư viện yêu cầu qua `pip`. Bạn có thể thực hiện điều này trong terminal hoặc command prompt của mình.

```bash
pip install opencv-python keras numpy matplotlib
Tải mô hình
Ứng dụng này yêu cầu hai mô hình học sâu đã huấn luyện:

Mô hình giới tính (gender_model.h5): Dự đoán giới tính của người trong ảnh.
Mô hình độ tuổi (age_model.h5): Dự đoán độ tuổi của người trong ảnh.
Hãy chắc chắn rằng bạn đã tải các mô hình này và lưu chúng trong thư mục phù hợp với mã nguồn của dự án.

Cách sử dụng
Chạy ứng dụng
Để chạy ứng dụng, bạn chỉ cần gọi hàm display_video() trong mã của bạn. Ứng dụng sẽ mở webcam của bạn và hiển thị kết quả dự đoán giới tính và độ tuổi trực tiếp.

python
Copy code
display_video()
Ứng dụng sẽ hiển thị ảnh từ webcam và hiển thị dự đoán về giới tính và tuổi ngay trên màn hình. Bạn có thể dừng ứng dụng bằng cách đóng cửa sổ hiển thị ảnh hoặc dừng chương trình bằng cách kiểm soát vòng lặp trong mã.

Mô tả về cách hoạt động
Xử lý ảnh đầu vào: Ảnh từ webcam được xử lý và chuyển sang dạng ảnh xám để phù hợp với yêu cầu đầu vào của mô hình.
Dự đoán giới tính: Mô hình giới tính sẽ phân loại người trong ảnh là "Nam" hoặc "Nữ".
Dự đoán tuổi: Mô hình độ tuổi sẽ đưa ra ước tính về độ tuổi của người trong ảnh.
Hiển thị kết quả: Kết quả sẽ được hiển thị ngay trên ảnh webcam và in ra console.
Các lưu ý
Mô hình yêu cầu ảnh đầu vào có kích thước cố định. Do đó, ảnh sẽ được thay đổi kích thước và chuẩn hóa trước khi đưa vào mô hình.
Ứng dụng này hoạt động tốt trên môi trường Python cục bộ với quyền truy cập webcam. Nếu bạn chạy trên Google Colab, bạn sẽ cần sử dụng một số thay đổi trong cách lấy ảnh từ webcam (như dùng eval_js để lấy ảnh webcam từ trình duyệt).
Các cải tiến trong tương lai
Tối ưu hóa mô hình cho việc dự đoán nhanh hơn trong môi trường trực tuyến.
Thêm tính năng phân tích cảm xúc và các đặc điểm khác từ khuôn mặt.
Tác giả
Tên tác giả: Vũ Hoài Nam
Email: 20212501@eaut.edu.vn
GitHub: https://github.com/vunameaut
Giấy phép


less
Copy code

### Các phần chính trong file `README.md`:

1. **Mô tả dự án**: Giới thiệu về mục tiêu và chức năng chính của dự án.
2. **Các yêu cầu**: Liệt kê các phần mềm và thư viện cần thiết để chạy ứng dụng.
3. **Cài đặt**: Hướng dẫn cài đặt các thư viện cần thiết.
4. **Cách sử dụng**: Hướng dẫn cách chạy ứng dụng và cách sử dụng các hàm trong mã nguồn.
5. **Các lưu ý**: Cung cấp thông tin quan trọng khi sử dụng dự án.
6. **Tác giả**: Thông tin về người phát triển dự án.
7. **Giấy phép**: Thông tin giấy phép của dự án.

File này giúp người khác dễ dàng hiểu được cách thiết lập và sử dụng dự án của bạn.