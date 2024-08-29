# Knowledge-Typescript

## 1. TypeScript là gì?
- TypeScript là siêu tập cú pháp của JavaScript (Superset Javascript), bổ sung thêm kiểu tĩnh.
- TypeScript là "Siêu tập cú pháp" có nghĩa là nó có cùng cú pháp cơ sở với JavaScript nhưng bổ sung thêm một số tính năng.
## 2. Cách cài đặt TypeScript?
> [!TIP]
> **Điều kiện: đã cài đặt visual studio code**
- [x] Setup Typescript (Window)  : **npm install -g typescript**
- [x] Setup Typescript (Mac)     : **sudo npm install -g typescript**
## 3. Tại sao nên sử dụng TypeScript?
- JavaScript là một ngôn ngữ có kiểu dữ liệu lỏng lẻo. Có thể khó hiểu loại dữ liệu nào đang được truyền trong JavaScript.
- Trong JavaScript, các tham số và biến hàm không có bất kỳ thông tin nào! Vì vậy, các nhà phát triển cần xem tài liệu hoặc đoán dựa trên việc triển khai.
- TypeScript cho phép chỉ định loại dữ liệu được truyền trong mã và có khả năng báo cáo lỗi khi các loại dữ liệu không khớp.
  
> Ví dụ, TypeScript sẽ báo lỗi khi truyền một chuỗi vào một hàm mong đợi một số. JavaScript thì không.
## 4. Các loại kiểu dữ liệu trong TypeScript
### 4.1. Kiểu dữ liệu cơ bản
+ Number: Đại diện cho cả số nguyên và số thực.
    ```
    let score: number = 100;  
    ```
+ String: Dữ liệu kiểu chuỗi.
    ```
    let greeting: string = "Hello, World!";  
    ```
+ Boolean: Giá trị đúng hoặc sai.
    ```
    let isActive: boolean = true;  
    ```
### 4.2. Các kiểu đặc biệt

+ Any: Chấp nhận bất kỳ kiểu dữ liệu nào.
    ```
    let variable: any = "Hello";  
    variable = 42; // Có thể gán các kiểu dữ liệu khác nhau  
    ```
+ Void: Thường được sử dụng cho các hàm không trả về giá trị nào.
    ```
    function log(message: string): void {  
        console.log(message);  
    }  
    ```
+ Null và Undefined: Đại diện cho giá trị không có và không được xác định.
### 4.3. Kiểu đối tượng
+ Object: Đại diện cho các đối tượng phức tạp.
    ```
    let employee: { name: string; age: number; position: string } = {  
        name: "John",  
        age: 25,  
        position: "Developer",  
    }; 
    ```
### 4.4. Mảng
+ Mảng có thể được định nghĩa với kiểu dữ liệu cụ thể.
    ```
    let numbers: number[] = [1, 2, 3, 4];  
    let names: Array<string> = ["Alice", "Bob"];  
    ```
### 4.5. Tuple
+ Tuple là mảng có số lượng phần tử cố định với các kiểu dữ liệu khác nhau.
    ```
    let user: [string, number] = ["Alice", 30];
    ```
### 4.6. Enum
+ Enum giúp định nghĩa một tập hợp các hằng số có tên.
    ```
    enum Direction {  
        Up,  
        Down,  
        Left,  
        Right,  
    }  
    ```
### 4.7. Union và Intersection Types
+ Union Types: Biến có thể mang nhiều kiểu khác nhau.
    ```
    function print(value: string | number) {  
        console.log(value);  
    }  
    ```
+ Intersection Types: Kết hợp nhiều kiểu thành một kiểu duy nhất.
    ```
    interface Person {  
        name: string;  
    }  
      
    interface Worker {  
        job: string;  
    }  
      
    type Employee = Person & Worker;  
    ```
## 5. Lợi ích khi sử dụng TypeScript
- Giảm thiểu lỗi thông qua việc kiểm tra kiểu tĩnh.
- Cải thiện khả năng bảo trì mã nguồn khi sử dụng cấu trúc mã rõ ràng và tổ chức tốt.
- Hỗ trợ phát triển nhanh chóng với các công cụ như autocompletion, điều này giúp lập trình viên phát hiện lỗi nhanh hơn.
## 6. Kết luận
- TypeScript là một ngôn ngữ mạnh mẽ, giúp lập trình viên xây dựng ứng dụng web dễ dàng và hiệu quả hơn với các tính năng nâng cao. Việc áp dụng TypeScript vào phát triển ứng dụng sẽ mang lại nhiều lợi ích cho người lập trình trong việc quản lý mã, kiểm soát lỗi và nâng cao chất lượng sản phẩm.
