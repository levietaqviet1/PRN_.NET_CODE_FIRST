# PRN_.NET_CODE_FIRST

# :notebook_with_decorative_cover: Table of Contents
- [Lý Thuyết](#Lý-Thuyết)
- [Quy ước](#Quy-ước)

## Lý Thuyết

- `Code-First` có nghĩa là trước tiên bạn cần bắt đầu viết mã bằng C# sau đó Entity Framework sẽ tạo cơ sở dữ liệu từ mã của bạn.

- Trong phương pháp Code-First, bạn tập trung vào miền ứng dụng của mình và bắt đầu tạo các lớp cho thực thể miền thay vì thiết kế cơ sở dữ liệu của bạn trước rồi tạo các lớp phù hợp với thiết kế cơ sở dữ liệu của bạn.

![image](https://user-images.githubusercontent.com/85175337/226838387-f12fe5dd-d3f9-4c81-a60e-18d6a5d36331.png)

- Quy trình làm việc Code-First

![image](https://user-images.githubusercontent.com/85175337/226838477-a8856862-3997-4d24-b4e6-e94255ec7d30.png)

![image](https://user-images.githubusercontent.com/85175337/226842646-516ca1a2-0164-4cdf-8068-1bae368da6a0.png)

## Quy ước

- `Table Name`: <Tên class> + 's'. Ví dụ class Student thì khi đặt tên ánh xạ sang DB thì nên đặt là Students 

- `Primary key Name`:  1 là để Id hoặc <Tên class> +"Id" điều đó là bắt buộc để khi biên dịch EF mới biết đâu là khóa chính. Nếu mà muốn đặt tên khóa chính khác với 2 cái trên thì thêm đánh dấu [Key] ở trước 

![image](https://user-images.githubusercontent.com/85175337/226841274-e07edf4b-7b39-4738-a1b1-30ccbf2edf40.png)

Trường hợp đánh 2 cặp khóa cho bảng trung gian để hỗ trợ cho mỗi quan hệ n-n thì có thể dùng PrimaryKey

![image](https://user-images.githubusercontent.com/85175337/226841597-765fe11b-5571-4761-b660-4fef434479e9.png)

![image](https://user-images.githubusercontent.com/85175337/226841685-9616a1f3-ea5e-4e6e-95f8-24c4b776978e.png)

- `Foreign key property Name`: 

![image](https://user-images.githubusercontent.com/85175337/226843405-e879ad25-7653-4e59-829d-4c098ed7ce33.png)

- `Null column`: EF tạo 1 cột có thể rỗng

- `DB Columns order`: Thứ tự cột sẽ được sinh ra trong table đó

![image](https://user-images.githubusercontent.com/85175337/226844958-2f37de99-d6ca-4023-a423-27f59fee95ee.png)


- `Kiểu dữ liệu khi chuyển sang`:

![image](https://user-images.githubusercontent.com/85175337/226842770-1b03ea57-6a2b-4f79-adb3-1fba14f8a969.png)

- `Cascade delete`: Tự động xóa các dữ liệu con

















