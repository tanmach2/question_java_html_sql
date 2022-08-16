# Question Java
1. Các thành phần chính trong Spring:
- Spring core container: 
- Spring ContextApplication Context:
- Spring AOP (Aspect-Oriented-programming):
- Spring DAO:
- Spring ORM:
- Spring web module:
- Spring MVC framework:


# Question SQL
1. transaction là gì? ví dụ thực tế hỏi có cách nào commit 1 phần transaction không?
- transaction là một tập hợp các phép thực thi (operation) xuống cơ sở dữ liệu một cách tuần tự với nguyên tắc một là thành công , hai là thất bại dù chỉ một operation và dữ liệu sẽ được trở lại (rollback) trạng thái ban đầu.
- các operation là phải được thực thi một cách độc lập, đang chạy operation này thì không được chạy operation khác.

- VÍ DỤ đơn giản là chuyển tiền từ A -> B:
+ nếu A bị trừ tiền và B nhận được tiền thì được coi là một transaction thành công.
+ nếu một trong hai thất bại thì được coi là thất bại và dữ liệu phải được rollback.

2. Các tính chất của Transaction.
 Có 4 tính chất ACID:
+ Atomicity (bảo toàn): một là thực hiện tất cả , hai là không làm gì cả nếu dù chỉ một lệnh không thành công.
+ consistency (nhất quán): dữ liệu từ khi bắt đầu cho đến khi kết thúc là phải nhất quán với nhau.
+ Isolation (cô lập): nếu có nhiều transaction cùng một lúc thì phải đảm bảo được các transaction là độc lập và không ảnh hưởng gì đến nhau trên dữ liệu.
+ Durability (bền vững): dữ liệu sau khi thực hiện transaction sẽ không được thay đối nếu gặp sự cố liên quan đến database.

3. câu lênh truy vấn của INNER JOIN và LEFT JOIN.
- SELECT A.title, B.first_name, B.last_name FROM movies AS A LEFT JOIN member AS B ON A.movies_id = B.id 
- SELECT A.title, B.first_name, B.last_name FROM movies AS A INNER JOIN member AS B ON A.movies_id = B.id 

4. Các loại bỏ các phần tử trùng lặp trong SQL.
- Sử dụng DISTINCT:

ví dụ: SELECT DISTINCT giatien FROM donHang ORDER BY giatien

- ORDER BY là câu lệnh sắp xếp tuần tự theo giá tiền. ASC là tăng dần và DESC là giảm dần.

5. Sự khác nhau giữa 
6. Những khó khăn trong dự án : ví dụ : requement không rõ ràng, công nghệ mới, 


# Question HTML CSS
1. sự khác nhau giữa === và ==? tại sao == lại chỉ so sánh giá trị?
- "===" là so sánh giá trị và cả kiểu dữ liệu còn "==" là chỉ so sánh giá trị. Tại vì khi sử dụng "==" thì một trong hai dữ liệu sẽ tự động chuyển đổi kiểu dữ liệu sao cho giống bên kia hoặc cả hai cùng nhau chuyển đổi sang một kiểu dữ liệu trung gian.

2. session và cookies khác nhau ở đâu và chúng được lưu ở đâu?
- session (phiên) là một bộ nhớ tạm thời được lưu trên mấy chủ , có bộ nhớ lên đến 5NB và sẽ mất khi hết thời gian chờ và đóng máy chủ hoặc trình duyệt.
- cookies là một bộ nhớ tạm thời được lưu trên máy client có dung lượng bộ nhớ là 4KB và chỉ lưu được trong một khoảng thời gian time.

3. Sự khác biệt giữa POST và GET.
- GET là phương thức truy xuất dữ liệu từ một tài nguyên được chỉ định và hiển thị trên thành địa chỉ URL nên nó không bảo mật so với POST.
- POST là phương thức cập nhập dữ liệu và không được hiển thị trên URL.
- GET chỉ chấp nhận các ký tự ASCII còn POST thì không bị ràng buộc.


4. jquery là gì? cú pháp để lấy nội dung phần tử HTML? AJAX là gì?
* jquery là một thư viện của javascript, giúp xây dựng các chức năng bằng javascript chở nên nhanh và dễ dàng hơn.