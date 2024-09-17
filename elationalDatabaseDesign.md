# Relational_Database_Design

## I. Giới thiệu chung

### 1. Database là gì?
- Cơ sở dữ liệu là nơi lưu trữ dữ liệu trên máy tính.
- Nó thường được lưu trữ trên các máy tính lớn gọi là máy chủ, Cơ sở dữ liệu chứa những thứ gọi là bảng
- Bảng là đối tượng dùng để lưu trữ dữ liệu. Một bảng giống như một bảng tính trong tệp bảng tính, như Excel hoặc Google Trang tính.
- Ví dụ DB về học sinh đơn giản:
  
   ![image](https://github.com/user-attachments/assets/1358572f-2a2e-4829-8644-509d110929d9)
### 2. Các loại Database
- Có 2 loại cơ sở dữ liệu:
  + cơ sở dữ liệu quan hệ (Đây là loại cơ sở dữ liệu chính được sử dụng trong các trang web và ứng dụng)
  + kho dữ liệu (Nó dựa trên một cái bàn trung tâm lớn với các bảng liên kết khác. Nó chủ yếu được sử dụng để báo cáo)
### 3. Lợi ích của Database
- Cơ sở dữ liệu quan hệ có nhiều lợi ích chẳng hạn như xóa thông tin trùng lặp cho phép cập nhật và xác thực định dạng dễ dàng.


## II. Quy trình mô hình hóa dữ liệu
> Quy trình mô hình hóa dữ liệu hiểu đơn giản là thu thập yêu cầu và từ yêu cầu đó chúng ta sẽ tiến hành thiết kế DB (bảng, quan hệ: 1-1,1-n,n-n, các ràng buộc, quy tắc, ...) dựa vào những yêu cầu đó.

### 1. Các bước mô hình hóa dữ liệu
- B1: Xác định mục tiêu của cơ sở dữ liệu
  + xác định mục tiêu của cơ sở dữ liệu giúp bạn xác định những gì cần lưu trữ.
  + Bạn cũng nên có một số loại phạm vi hoặc ranh giới cho những gì bạn muốn hoặc những gì bạn cần lưu trữ.
  + hành động này là trả lời câu hỏi về cơ sở dữ liệu của bạn: > Mục tiêu của cơ sở dữ liệu là gì? và nó đang cố gắng đạt được điều gì?
- B2: Xem xét hệ thống hiện tại
  > Trả lời được những câu hỏi: 
  + Có hệ thống hiện hành không?
  + Dữ liệu của hệ thống hiện tại được lưu trữ như thế nào?
  + Nó hoạt động tốt như thế nào?
  + Những vấn đề với hệ thống hiện tại là gì?
  + Dữ liệu như thế nào?
- B3: Thu thập yêu cầu của cơ sở dữ liệu
  + tìm hiểu xem bạn cần nói chuyện với ai, tìm hiểu thông tin nào cần được lưu trữ, và tìm hiểu xem có cần lưu trữ lịch sử thay đổi hay không.
- B4: Tìm kiếm ngoại lệ cho các quy tắc
  + Các hành động dành cho từng yêu cầu của bạn xác định nếu có bất kỳ ngoại lệ nào đối với các quy tắc, và đặt câu hỏi về bất kỳ độ dài trường cụ thể nào hoặc các hạn chế về loại vì chúng có thể cần phải được tăng lên trong tương lai.
- B5: Nhận dạng các thực thể
  + Xác định danh từ trong câu. Chuyển đổi chúng thành các thực thể bằng cách loại bỏ các bản sao và chuyển chúng sang dạng số ít.
- B6: Xác định các thuộc tính
  + thuộc tính là thứ được lưu trữ cho mỗi thực thể. Có thể đó sẽ là một cột hoặc một trường trong cơ sở dữ liệu.

## III. Thiết kế Database

### 1. Chuẩn hóa 
- Dạng chuẩn hóa 1: Xác định Khóa chính
- Dạng chuẩn hóa 2: Xác định khóa ngoại và attribute
- Dạng chuẩn hóa 3: Xác định quan hệ (1-1, 1-n, n-1, n-n)


## IV. Những lưu ý khi thiết kế Database
- Kiểu dữ liệu và độ chính xác (Chú ý độ dài của dữ liệu nó có thể sai ở tương lai)
- Ràng buộc toàn vẹn (xem xét từng trường trong cơ sở dữ liệu của bạn, xác định xem bạn có cần hạn chế chúng theo cách nào đó không Ví dụ như: giá trị NULL)
-  Quy ước đặt tên (Hãy quy ước đặt tên bảng, trường, .. từ lúc bắt đầu thể hiện sự nhất quán cho Database của bạn)
-  Bảng tra cứu và kiểm toán (Nó cũng được gọi là bảng tham chiếu, Nó được tìm kiếm cho nhiều mục đích khác nhau và nó thường là một bảng độc lập không liên kết với các bảng khác)
-  Kiểm toán bảng (Bảng kiểm toán lưu giữ lịch sử thay đổi của một bảng, Nó được thực hiện bằng cách sử dụng logic cơ sở dữ liệu, hoặc thậm chí là hệ thống sử dụng bảng) 


