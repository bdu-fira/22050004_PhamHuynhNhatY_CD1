BỘ GIÁO DỤC VÀ ĐÀO TẠO
TRƯỜNG ĐẠI HỌC BÌNH DƯƠNG
KHOA CÔNG NGHỆ THÔNG TIN, 
ROBOT VÀ TRÍ TUỆ NHÂN TẠO

 


TIỂU LUẬN KẾT THÚC MÔN HỌC
CHUYÊN ĐỀ 1



Tên đề tài:
THIẾT KẾ WEB BÁN ĐỒ CHƠI


Giảng viên hướng dẫn: ThS. Nguyễn Thanh Sơn
ThS. Hồ Ngọc Giàu
ThS. Dương Anh Tuấn
ThS. Nguyễn Hữu Quyền
Sinh viên thực hiện: 
1. 22050004 – PHẠM HUỲNH NHẬT Ý – 25TH02
2. 22050010 – ĐỖ HỮU TRÍ – 25TH02
3. 22050089 – PHẠM HỒNG QUÝ – 25TH02



Bình Dương, tháng 04 năm 2025  
NHẬN XÉT VÀ CHẤM ĐIỂM CỦA GIẢNG VIÊN
TIỂU LUẬN MÔN: CHUYÊN ĐỀ 1
1.	Nhận xét:
a)	Những kết quả đạt được:
	
	
	
	
	
b)	Những hạn chế:
	
	
	
	
	
2.	Điểm đánh giá (Ghi rõ thông tin sinh viên và điểm chữ, điểm số) 
	
	
	
	
	
	


	Bình Dương, ngày  …  tháng  … năm 2025
Giảng viên chấm thi
(Ký và ghi rõ họ tên)




MỤC LỤC
NHẬN XÉT VÀ CHẤM ĐIỂM CỦA GIẢNG VIÊN	I
CHƯƠNG 1: GIỚI THIỆU ĐỀ TÀI	1
1.	Mục tiêu	1
1.1	Mục tiêu chính:	1
1.2	Mục tiêu cụ thể:	1
2.	Ý nghĩa	1
3.	Phương pháp thực hiện	2
4.	Kế hoạch thực hiện & phân công công việc	3
CHƯƠNG 2: PHÂN TÍCH HỆ THỐNG	5
1.	Biểu đồ use-case	5
2.	Đặc tả use case	6
3.	Sơ đồ lớp	11
4.	Các sơ đồ động	12
CHƯƠNG 3: THIẾT KẾ HỆ THỐNG	14
1.	Sơ đồ logic dữ liệu	14
2.	Mô tả chi tiết các bảng dữ liệu	14
3.	Sơ đồ giao diện hệ thống	17
4.	Một số giao diện	18
CHƯƠNG 4: HIỆN THỰC HỆ THỐNG	25
1.	Kiến trúc hệ thống	25
2.	Lập trình hiện thực chức năng	25
3.	Kiểm thử	27
CHƯƠNG 5: TỔNG KẾT	29
1.	Kết quả đạt được	29
2.	Hạn chế và kinh nghiệm	29
TÀI LIỆU THAM KHẢO	31

 
DANH MỤC BẢNG BIỂU
Bảng 1.4.1 Kế hoạch thực hiện	3
Bảng 1.4.2 Phân công công việc	4
Bảng 2.2.1 Đặc tả use case – Đăng nhập	7
Bảng 2.2.2 Đặc tả use case – Đăng ký	7
Bảng 2.2.3 Đặc tả use case –Đánh giá của khách hàng khi mua hàng	8
Bảng 2.2.4 Đặc tả use case –Cập nhật sản phẩm	8
Bảng 2.2.5 Đặc tả use case – Quên mật khẩu	9
Bảng 2.2.6 Đặc tả use case – Tìm kiếm	10
Bảng 2.2.7 Đặc tả use case – Xem sản phẩm	10
Bảng 2.2.8 Đặc tả use case – Xem lịch sử hoạt động của trang web	11
Bảng 3.2.1 Chi tiết bảng dữ liệu	16
 
DANH MỤC HÌNH ẢNH
Hình 2.1.1: Biểu đồ use - case của Khách hàng	5
Hình 2.1.2: Biểu đồ use - case của Admin	5
Hình 2.1.3: Biểu đồ use - case của nhân viên	6
Hình 2.3.1: Sơ đồ lớp	11
Hình 2.3.2: Sơ đồ hoạt động của các quy trình chính	12
Hình 2.3.3: Sơ đồ tuần tự đơn giản cho đặt hàng	13
Hình 3.1.1: Sơ đồ logic dữ liệu	14
Hình 3.3.1 Sơ đồ giao diện hệ thống	18
Hình 3.4.1 Trang chủ	18
Hình 3.4.2 Sản phẩm mới nhất	19
Hình 3.4.3 Giới thiệu	19
Hình 3.4.4 Đăng nhập	20
Hình 3.4.5 Giỏ hàng	21
Hình 3.4.6 thông tin tài khoản	21
Hình 3.4.7 Thông tin liên hệ	22
Hình 3.4.8 Thống kê doanh thu - Admin	22
Hình 3.4.9 Thông tin sản phẩm – Admin	22
Hình 3.4.10 Loại sản phẩm - Admin	23
Hình 3.4.11 Hóa đơn - Admin	23
Hình 3.4.12 Danh mục sản phẩm - Admin	23
Hình 3.4.13 Thông tin tài khoản người dùng	24
Hình 4.2.1 Mã nguồn kết nối cơ sở dữ liệu	25
Hình 4.2.2 Mã nguồn trang thanh toán đơn hàng	26
Hình 4.2.3 Mã nguồn trang đăng nhập	27
Hình 4.2.4 Mã nguồn trang danh sách tài khoản user của Admin	27
Hình 4.3.1 Đăng ký và đăng nhập	28
Hình 4.3.2 Đăng ký tài khoản thành công	28

 
 
1.1. GIỚI THIỆU ĐỀ TÀI
"Website bán đồ chơi trẻ em" quản lý các thông tin về sản phẩm bao gồm đồ chơi giáo dục, đồ chơi vận động, đồ chơi thông minh và các phụ kiện kèm theo.
Website quản lý nhiều sản phẩm. Mỗi sản phẩm có mã sản phẩm, tên sản phẩm, giá, thông số, hình ảnh, khuyến mãi, số lượng, màu sắc... và chỉ thuộc một loại sản phẩm, thông tin về loại sản phẩm bao gồm mã loại sản phẩm, tên loại sản phẩm. Mỗi loại sản phẩm sẽ có các hãng sản xuất và các thông số tương ứng. Thông tin về thông số bao gồm mã thông số, tên thông số. Mỗi sản phẩm sẽ chứa nhiều thông số và chỉ thuộc về một hãng sản xuất. Thông tin về hãng sản xuất bao gồm mã hãng sản xuất, tên hãng sản xuất.
Người dùng ghé thăm website và muốn mua sản phẩm sẽ phải cung cấp các thông tin bao gồm: họ tên, số điện thoại, ngày sinh, email... Người dùng sau khi đăng nhập sẽ trở thành thành viên của website và được phép lập đơn đặt hàng. Thông tin về đơn đặt hàng gồm mã đơn đặt hàng, mã thành viên, tổng tiền, mã trạng thái, ngày lập. Mỗi đơn đặt hàng sẽ thuộc một trạng thái nhất định, trạng thái đơn đặt hàng bao gồm mã trạng thái, tên trạng thái.
Mỗi người dùng khi đăng nhập vào website sẽ được cấp một quyền nhất định. Thông tin quyền gồm mã quyền, tên quyền.
Website cũng cho phép người dùng theo dõi các tin tức về khuyến mãi, các hoạt động cho trẻ em, hướng dẫn giáo dục... Thông tin về tin tức bao gồm mã tin tức, tên tin tức, hình ảnh, ngày đăng, tóm tắt, nội dung. Mỗi tin tức sẽ thuộc một loại tin tức, loại tin tức bao gồm mã loại tin tức, tên loại tin tức. Ngoài ra website cũng cung cấp thêm chức năng hỗ trợ trực tuyến, thông tin hỗ trợ bao gồm mã hỗ trợ, mã thành viên, hình ảnh.
1.2. MỤC ĐÍCH CỦA ĐỀ TÀI
– Xây dựng một website giúp phụ huynh dễ dàng theo dõi thông tin của sản phẩm đồ chơi, tin tức về hoạt động giáo dục, phát triển kỹ năng cho trẻ em.
– Là một website bán hàng trực tuyến nên việc trình bày sản phẩm phải rõ ràng, thu hút được người xem và dễ dàng sử dụng.
– Các sản phẩm mới hoặc thông tin về khuyến mãi của cửa hàng cần có dấu hiệu kích thích thu hút người dùng truy cập.
– Dữ liệu trong website được load nhanh chóng và chính xác.
– Ban quản trị có thể kiểm soát được các thông tin của website và đảm bảo việc quản lý các thông tin phải nhanh chóng và chính xác.
– Cung cấp giao diện thân thiện và dễ sử dụng cho người dùng, đặc biệt chú trọng đến trải nghiệm tìm kiếm và lựa chọn đồ chơi theo nhu cầu, độ tuổi và mục đích giáo dục.
1.3. PHẠM VI ĐỀ TÀI
MVC là phương pháp chia nhỏ một ứng dụng thành ba phần để cài đặt, mỗi thành phần đóng vai trò khác nhau và ảnh hưởng lẫn nhau gồm: Models, Views và Controllers. Nền tảng Node.js với Express MVC có đặc điểm nổi bật là nhẹ, dễ kiểm thử phần giao diện, hiệu suất cao và khả năng xử lý bất đồng bộ tốt.
Models: là một phần của ứng dụng, các đối tượng này thiết lập logic của phần dữ liệu của ứng dụng. Thông thường, các đối tượng model lấy và lưu trạng thái của model trong CSDL.
Views: là các thành phần dùng để hiển thị giao diện người dùng (UI). Thông thường, view được tạo dựa vào thông tin dữ liệu model.
Controllers: là các thành phần dùng để quản lý tương tác người dùng, làm việc với model và chọn view để hiển thị giao diện người dùng. Trong một ứng dụng MVC, view chỉ được dùng để hiển thị thông tin, controller chịu trách nhiệm quản lý và đáp trả nội dung người dùng nhập và tương tác với người dùng.
Lợi ích của ứng dụng web dựa trên mô hình MVC:
Dễ dàng quản lý sự phức tạp của ứng dụng bằng cách chia ứng dụng thành ba thành phần model, view, controller.
Phân tách rõ ràng giữa logic xử lý và giao diện người dùng, giúp việc phát triển và bảo trì dễ dàng hơn.
Hỗ trợ tốt cho các ứng dụng được xây dựng bởi những đội có nhiều lập trình viên và thiết kế mà vẫn quản lý được tính năng của ứng dụng.
Dễ dàng mở rộng và nâng cấp trong tương lai với cấu trúc rõ ràng.
Hệ thống là một ứng dụng website được xây dựng trên nền công nghệ Node.js, kết hợp với công nghệ AJAX nhằm nâng cao hiệu suất hoạt động và tốc độ xử lý, sử dụng hệ quản trị CSDL trên MySQL. Frontend được phát triển bằng HTML, CSS và JavaScript hiện đại, tạo trải nghiệm người dùng mượt mà và thân thiện.
3.	Phương pháp thực hiện
Khảo sát hiện trạng:
­	Thu thập thông tin về nhu cầu người dùng và phân tích các hệ thống website bán hàng hiện có trên thị trường.
­	Đánh giá các tính năng, ưu nhược điểm của các website đối thủ để xác định các yêu cầu cần thiết cho hệ thống mới.
Xác định yêu cầu và sử dụng biểu đồ Use Case:
­	Thu thập các yêu cầu chức năng và phi chức năng thông qua khảo sát người dùng và phân tích thị trường.
­	Sử dụng biểu đồ Use Case để mô hình hóa các yêu cầu, xác định các tác nhân (actors) và các trường hợp sử dụng (use cases), giúp làm rõ các luồng tương tác chính giữa người dùng và hệ thống.
Thiết kế cơ sở dữ liệu bằng XAMPP:
­	Sử dụng XAMPP tích hợp phpMyAdmin để thiết kế cơ sở dữ liệu, xây dựng các bảng và mối quan hệ giữa chúng, phục vụ cho việc lưu trữ thông tin sản phẩm, khách hàng, đơn hàng.
­	Tối ưu hóa cấu trúc cơ sở dữ liệu để đảm bảo hiệu suất truy xuất và tính toàn vẹn dữ liệu.
Thiết kế giao diện người dùng và xử lý Backend bằng PHP:
­	Thiết kế giao diện người dùng (UI) theo các nguyên tắc thiết kế UX, đảm bảo thân thiện và dễ sử dụng trên cả thiết bị di động và máy tính.
­	Phát triển các chức năng chính của hệ thống như quản lý sản phẩm, giỏ hàng, thanh toán, và quản lý người dùng bằng PHP cho phần backend, đảm bảo xử lý yêu cầu từ người dùng một cách nhanh chóng và chính xác.
Xây dựng, kiểm thử và triển khai hệ thống:
­	Xây dựng từng module theo thiết kế, kiểm thử từng phần và tích hợp toàn bộ hệ thống.
­	Tiến hành kiểm thử chức năng (Functional Testing), kiểm thử hiệu năng (Performance Testing) để đảm bảo hệ thống hoạt động ổn định.
­	Triển khai website trên môi trường máy chủ thực tế, thực hiện kiểm tra cuối cùng trước khi đưa vào sử dụng.
4.	Kế hoạch thực hiện & phân công công việc
	Kế hoạch thực hiện
Giai đoạn
Nội dung công việc	Thời gian thực hiện

1. Khảo sát và phân tích yêu cầu	
- Thu thập yêu cầu từ khách hàng
- Nghiên cứu thị trường và các hệ thống tương tự
- Mô hình hóa yêu cầu bằng biểu đồ Use Case	1 tuần
2. Thiết kế hệ thống	- Thiết kế cơ sở dữ liệu bằng Mariadb
- Thiết kế giao diện người dùng (UI/UX)
- Lên sơ đồ kiến trúc hệ thống	4 tuần
3. Phát triển và lập trình backend	- Lập trình các chức năng backend bằng PHP
- Xây dựng chức năng quản lý sản phẩm, giỏ hàng, người dùng	3 tuần
4. Tích hợp và kiểm thử	- Tích hợp các module lại với nhau
- Thực hiện kiểm thử chức năng, hiệu năng
- Sửa lỗi và tối ưu hóa	2 tuần
5. Triển khai và nghiệm thu	- Triển khai website lên máy chủ
- Kiểm thử lần cuối
- Thu thập phản hồi và điều chỉnh nếu cần thiết	1 tuần
Bảng 1.4.1 Kế hoạch thực hiện

Thời gian dự kiến hoàn thành: Khoảng 11 tuần.

 
Phân công công việc 
Công việc	Đỗ Hữu Trí	Phạm Huỳnh Nhật Ý	Phạm Hồng Quý
1. Khảo sát và phân tích yêu cầu	- Khảo sát yêu cầu xử lý từ phía máy chủ
- Lập danh sách API cần thiết	- Phân tích cấu trúc dữ liệu
- Lập kế hoạch xây dựng CSDL
	- Khảo sát giao diện người dung
- Lập danh sách các tính năng tương tác
2. Thiết kế hệ thống	- Thiết kế kiến trúc backend
- Xây dựng luồng xử lý dữ liệu	- Thiết kế cơ sở dữ liệu bằng MySQL
- Lên sơ đồ ERD và kiến trúc CSDL
- Thiết kế các bảng và mối quan hệ	- Thiết kế giao diện người dùng (UI/UX)
- Xây dựng wirefram
3. Phát triển và lập trình backend	- Lập trình backend bằng Node.js
- Xây dựng API cho các chức năng
- Xử lý logic nghiệp vụ
- Xử lý bảo mật	- Xây dựng và quản lý CSDL
- Viết stored procedures và queries
- Tối ưu hóa truy vấn	- Phát triển các chức năng frontend
- Lập trình giao diện với HTML, CSS, JavaScript
- Xử lý tương tác người dung 
4. Tích hợp và kiểm thử	- Tích hợp API với frontend
- Kiểm thử các API và xử lý lỗi
- Xử lý kết nối CSDL	- Kiểm thử hiệu suất CSDL
- Kiểm tra tính toàn vẹn dữ liệu
- Sửa lỗi và tối ưu truy vấn	- Kiểm thử giao diện người dung
- Đảm bảo tương thích đa trình duyệt
- Sửa lỗi và tối ưu hi
5. Triển khai và nghiệm thu	- Cấu hình và triển khai backend Node.js lên máy chủ
- Cài đặt môi trường thực thi
- Viết tài liệu API	- Triển khai CSDL lên máy chủ
- Thiết lập sao lưu và phục hồi dữ liệu
- Kiểm tra bảo mật CSDL	- Triển khai frontend lên máy chủ
- Thu thập phản hồi từ người dung
- Điều chỉnh và tối ưu giao diện
Bảng 1.4.2 Phân công công việc 



 
CHƯƠNG 2: PHÂN TÍCH HỆ THỐNG
1.	Biểu đồ use-case
 
Hình 2.1.1: Biểu đồ use - case của Khách hàng


 
Hình 2.1.2: Biểu đồ use - case của Admin


 
Hình 2.1.3: Biểu đồ use - case của nhân viên

 
Hình 2.1.4: Biểu đồ use - case tổng quát

2.	Đặc tả use case
Đăng nhập
1.	Mô tả tóm tắt:
-	Mã UC:
-	Tên UC: đăng nhập
-	Mục đích: giúp người dùng đăng nhập vào hệ thống
-	Tác nhân: Tất cả tác nhân có tài khoản trên hệ thống
-	Mô tả tóm lược: UC này bắt đầu khi tác nhân nhấn/click vào nút/biểu tượng đăng nhập trên trang chủ. (web)
-	Ngày:
-	Phiên bản: [Phiên bản hiện tại]
-	Người lập (người đặc tả):
2.	Dòng sự kiện chính:
B2.1: Tác nhân nhập vào tên đăng nhập và mật khẩu
B2.2: Tác nhân nhấn enter hoặc click vào biểu tượng/nút đăng nhập
B2.3:  Hệ thống kiểm tra thông tin đăng nhập, xử lý và thông báo kết quả
3.	Dòng sự kiện phụ:
-	Tại bước B2.1 nếu người dùng nhập thiếu thông tin thì hệ thống sẽ thông báo và yêu cầu nhập đầy đủ.
-	Tại bước B2.3 nếu người dùng nhập sai thông tin quá 3 lần thì hệ thống sẽ tạm khóa tài khoản.
4.	Tiền điều kiện:  Hệ thống đang ở trạng thái đã có tài khoản đã đăng ký trước đó của người dùng đang thao tác.
5.	Hậu điều kiện:
Nếu đăng nhập thành công:
-	Hệ thống sẽ hiển thị thông báo “Đăng nhập thành công” và chuyển đến trang chủ.
Bảng 2.2.1 Đặc tả use case – Đăng nhập

Đăng ký
Tên UC: Đăng ký
Mục đích: Admin tạo tài khoản cho nhân viên, khách hàng tạo tài khoản
Tóm lược: UC bắt đầu khi khách hàng hoặc admin truy cập vào trang đăng ký và điền thông tin.
Tác nhân: Admin, khách hàng
Ngày lập: [Điền ngày]
Phiên bản: [Phiên bản hiện tại]
Dòng sự kiện chính:
1.	Yêu cầu người dùng điền thông tin cá nhân.
2.	Người dùng nhập các thông tin như họ tên, email, mật khẩu.
3.	Hệ thống kiểm tra tính hợp lệ của thông tin.
4.	Nếu thông tin hợp lệ, tạo tài khoản cho người dùng.
5.	Thông báo kết quả cho người dùng.
Dòng sự kiện phụ:
Nếu thông tin không hợp lệ, thông báo cho người dùng và yêu cầu nhập lại.

Tiền điều kiện:
1.	Hệ thống có sẵn giao diện đăng ký.
2.	Người dùng chưa có tài khoản trong hệ thống.
Hậu điều kiện:
1.	Tài khoản của người dùng được tạo thành công.
2.	Hệ thống sẵn sàng cho người dùng thực hiện các thao tác khác.
Bảng 2.2.2 Đặc tả use case – Đăng ký


Đánh giá của khách hàng khi đã mua hàng
•	Tên UC: Đánh giá sản phẩm
•	Mục đích: Khách hàng có thể để lại đánh giá về sản phẩm sau khi mua.
•	Tóm lược: Bắt đầu khi khách hàng đã mua hàng và chọn mục đánh giá sản phẩm.
•	Tác nhân: Khách hàng
•	Ngày lập: [Điền ngày]
•	Phiên bản: [Phiên bản hiện tại]
Dòng sự kiện chính:
1.	Khách hàng chọn sản phẩm đã mua và nhập đánh giá.
2.	Khách hàng nhập số sao (từ 1-5) và bình luận về sản phẩm.
3.	Hệ thống lưu lại đánh giá và hiển thị trên trang sản phẩm.
Dòng sự kiện phụ:
Nếu không có sản phẩm nào đủ điều kiện để đánh giá, hệ thống thông báo lỗi.

Tiền điều kiện:
Khách hàng phải đã mua sản phẩm.

Hậu điều kiện:
Đánh giá của khách hàng được lưu và hiển thị trên trang sản phẩm.


Bảng 2.2.3 Đặc tả use case –Đánh giá của khách hàng khi mua hàng

Cập nhật sản phẩm
•	Tên UC: Cập nhật sản phẩm
•	Mục đích: Admin cập nhật thông tin sản phẩm.
•	Tóm lược: Bắt đầu khi admin chọn chức năng cập nhật thông tin sản phẩm từ trang quản lý.
•	Tác nhân: Admin
•	Ngày lập: [Điền ngày]
•	Phiên bản: [Phiên bản hiện tại]
Dòng sự kiện chính:
1.	Admin chọn sản phẩm cần cập nhật.
2.	Admin nhập thông tin mới như giá cả, mô tả, hình ảnh sản phẩm.
3.	Hệ thống lưu thông tin cập nhật và hiển thị trên trang sản phẩm.
Dòng sự kiện phụ:
Nếu có lỗi trong quá trình cập nhật, hệ thống thông báo cho admin.

Tiền điều kiện:
Hệ thống phải có sẵn sản phẩm để admin có thể cập nhật.

Hậu điều kiện:
Thông tin sản phẩm được cập nhật thành công và hiển thị đúng trên trang.

Bảng 2.2.4 Đặc tả use case –Cập nhật sản phẩm


Quên mật khẩu
•	Tên UC: Quên mật khẩu
•	Mục đích: Cấp lại khẩu mới.
•	Tóm lược: Bắt đầu khi khách hàng/nhân viên chọn chức năng quên mật khẩu từ trang đăng nhập.
•	Tác nhân: Khách hàng, nhân viên, Admin
•	Ngày lập: [Điền ngày]
•	Phiên bản: [Phiên bản hiện tại]
Dòng sự kiện chính:
1.	Khách hàng hoặc nhân viên click vào nút Quên mật khẩu.
2.	Điền thông tin tài khoản cần cấp lại mật khẩu.
3.	Hệ thống lưu lịch sử tài khoản và gửi mật khẩu mặt định đến hòm thư của Gmail/Số điện thoại/Tài khoản liên kết.

Dòng sự kiện phụ:
Nếu nhập sai thông tin tài khoản cần tạo lại mật khẩu quá nhiều lần, hệ thống thông báo cho admin.

Tiền điều kiện:
Hệ thống phải có sẵn tài khoản cần tạo lại mật khẩu.

Hậu điều kiện:
Sau khi nhập mật khẩu mới được cấp từ hệ thống, bắt buộc người dùng phải thay đổi mật khẩu lần đầu để bảo mật tài khoản.

Bảng 2.2.5 Đặc tả use case – Quên mật khẩu
Tìm kiếm
•	Tên UC: Tìm kiếm
•	Mục đích: Tìm sản phẩm.
•	Tóm lược: Bắt đầu khi khách hàng, nhân viên hay admin chọn chức năng tìm kiếm.
•	Tác nhân: Khách hàng, nhân viên, Admin
•	Ngày lập: [Điền ngày]
•	Phiên bản: [Phiên bản hiện tại]
Dòng sự kiện chính:
1.	Người dùng nhập sản phẩm muốn tìm kiếm vào ô tìm kiếm.
2.	Click vào nút tìm kiếm để hệ thống đưa ra các sản phẩm cần tìm
3.	Hệ thống sẽ hiển thị những sản phẩm cần tìm và các sản phẩm liên quan (nếu có).
Dòng sự kiện phụ:
Không có.
Tiền điều kiện:
Hệ thống phải có sẵn sản phẩm để hiển thị khi nhận yêu cầu tìm kiếm.

Hậu điều kiện:
Thông tin sản phẩm được hiển thị đúng trên trang.

Bảng 2.2.6 Đặc tả use case – Tìm kiếm

Xem sản phẩm
•	Tên UC: Xem sản phẩm
•	Mục đích: Xem thông tin sản phẩm.
•	Tóm lược: Bắt đầu khi khách hàng click vào sản phẩm.
•	Tác nhân: Khách hàng, nhân viên, Admin
•	Ngày lập: [Điền ngày]
•	Phiên bản: [Phiên bản hiện tại]
Dòng sự kiện chính:
1.	Khách hàng hoặc Nhân viên/admin click chuột sản phẩm muốn xem.
2.	Hệ thống chuyển đến trang thông tin chi tiết sản phẩm.
Dòng sự kiện phụ:
Không có.
Tiền điều kiện:
Hệ thống phải có sẵn sản phẩm để hiển thị.

Hậu điều kiện:
Thông tin chi tiết sản phẩm được hiển thị đúng trên trang.

Bảng 2.2.7 Đặc tả use case – Xem sản phẩm

Xem lịch sử hoạt động của trang web
•	Tên UC: Xem lịch sử hoạt động của trang web
•	Mục đích: Quản lý trang web.
•	Tóm lược: Bắt đầu khi nhân viên hay admin chọn chức năng Xem lịch sử hoạt động trong.
•	Tác nhân: Admin
•	Ngày lập: [Điền ngày]
•	Phiên bản: [Phiên bản hiện tại]
Dòng sự kiện chính:
1.	Admin click vào xem lịch sử hoạt động.
2.	Chọn nhân viên hoặc khách hàng cần xem lại lịch sử hoạt động
3.	Hệ thống sẽ hiển thị những hoạt động mà nhân viên hoặc khách hàng đã thực hiện
Dòng sự kiện phụ:
Admin có thể xem lịch sử hoạt động tổng thể của trang web.
Tiền điều kiện:
Hệ thống phải lưu mọi hoạt động của khách hàng/nhân viên.

Hậu điều kiện:
Hiển thị lịch sử hoạt động của khách hàng, nhân viên.
Bảng 2.2.8 Đặc tả use case – Xem lịch sử hoạt động của trang web

3.	Sơ đồ lớp
 
Hình 2.3.1: Sơ đồ lớp
 
4.	Các sơ đồ động
 
Hình 2.3.2: Sơ đồ hoạt động của các quy trình chính

 
Hình 2.3.3: Sơ đồ tuần tự đơn giản cho đặt hàng
 
Hình 2.3.4: Sơ đồ tuần tự đơn giản cho bán hàng 
CHƯƠNG 3: THIẾT KẾ HỆ THỐNG
1.	Sơ đồ logic dữ liệu
 
Hình 3.1.1: Sơ đồ logic dữ liệu

2.	Mô tả chi tiết các bảng dữ liệu

1. Bảng TaiKhoan (Quản lý admin)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_admin	INT	Khóa chính	Mã định danh admin
2	Ten_admin	VARCHAR(100)	NOT NULL	Tên của admin
3	Email	VARCHAR(100)	NOT NULL	Email đăng nhập
4	So_dien_thoai	VARCHAR(20)		Số điện thoại liên hệ
5	Quyen_han	VARCHAR(50)	NOT NULL	Phân quyền của admin

2. Bảng LoaiSP (Phân loại sản phẩm)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_loai_san_pham	INT	Khoá chính	Mã loại sản phẩm
2	Ten_loai_san_pham	VARCHAR(100)	NOT NULL	Tên loại sản phẩm
3	Mo_ta_loai_san_pham	TEXT		Mô tả về loại sản phẩm
4	Ngay_tao	DATATIME	DEFAULT NOW()	Ngày tạo loại sản phẩm

3. Bảng SanPham (Thông tin sản phẩm)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_san_pham	INT	Khóa chính	Mã sản phẩm
2	Ten_ma_san_pham	VARCHAR(200)	NOT NULL	Tên của sản phẩm
3	Mo_ta	TEXT		Mô tả sản phẩm
4	Gia_ban	DOUBLE	NOT NULL	Giá bán sản phẩm
5	So_luong_ton_kho	INT	NOT NULL, DEFAULT 0	Số lượng còn trong kho
6	ID_loai_san_pham	INT	Khóa ngoại	Mã loại sản phẩm
7	ID_KM	INT	NULL	Mã khuyến mãi của sản phẩm

4. Bảng KhachHang (Thông tin khách hàng)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_khach_hang	INT	Khoá chính	Mã khách hàng
2	Ten_khach_hang	VARCHAR(100)	NOT NULL	Tên khách hàng
3	Dia_chi_giao_hang	TEXT	NOT NULL	Địa chỉ giao hàng
4	So_dien_thoai	VARCHAR(20)	NOT NULL	Số điện thoại liên hệ

5. Bảng DonHang (Thông tin đơn hàng)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_don_hang	INT	Khoá chính	Mã đơn hàng
2	Ngay_tao_don_hang	DATETIME	DEFAULT NOW()	Ngày tạo đơn
3	Trang_thai_don_hang	VARCHAR(50)	NOT NULL	Trạng thái đơn hàng
4	Tong_gia_tri	DOUBLE	NOT NULL	Tổng giá trị đơn hàng
5	ID_khach_hang	INT	Khóa ngoại	Mã khách hàng


6. Bảng ChiTietDonHang (Chi tiết từng sản phẩm trong đơn)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_chi_tiet_don_hang	INT	Khóa chính	Mã chi tiết đơn hàng
2	ID_don_hang	INT	Khóa ngoại	Mã đơn hàng
3	ID_san_pham	INT	Khóa ngoại	Mã sản phẩm
4	So_luong_san_pham	INT	NOT NULL	Số lượng mua
5	Gia_ban_san_pham	DOUBLE	NOT NULL	Giá bán tại thời điểm mua
6	Tong_gia	DOUBLE	NOT NULL	Tổng giá = Số lượng* Giá bán


7. Bảng HinhThucThanhToan (Quản lý thanh toán)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_thanh_toan	INT	Khóa chính	Mã thanh toán
2	Phuong_thuc_thanh_toan	VARCHAR(100)	NOT NULL	Phương thức thanh toán
3	Trang_thai_thanh_toan
	VARCHAR(50)	NOT NULL	Trạng thái thanh toán
4	So_tien_thanh_toan	DOUBLE	NOT NULL	Số tiền thanh toán
5	ID_don_hang	INT	Khóa ngoại	Mã đơn hàng

Bảng 3.2.1 Chi tiết bảng dữ liệu

Chi tiết các bảng và khóa:
Bảng USERS:
Khóa chính (PK): user_id
Khóa unique (UK): username, email
Không có khóa ngoại
Bảng CATEGORIES:
Khóa chính (PK): category_id
Không có khóa ngoại
Bảng PRODUCTS:
Khóa chính (PK): product_id
Khóa ngoại (FK): category_id -> liên kết với CATEGORIES
Bảng ORDERS:
Khóa chính (PK): order_id
Khóa ngoại (FK): user_id -> liên kết với USERS
Bảng ORDER_DETAILS:
Khóa chính (PK): order_detail_id
Khóa ngoại (FK): 
order_id -> liên kết với ORDERS
product_id -> liên kết với PRODUCTS
Các đặc điểm bổ sung:
Thêm các trường timestamp (created_at, updated_at) để theo dõi thời gian
Thêm trường status cho đơn hàng
Thêm trường is_active cho sản phẩm
Thêm trường is_paid cho đơn hàng
Các trường decimal cho các giá trị tiền tệ
Các ràng buộc unique cho username và email
Mối quan hệ chính:
Users (1) - (n) Orders
Categories (1) - (n) Products
Products (1) - (n) Order_Details
Orders (1) - (n) Order_Details


 
3.	Sơ đồ giao diện hệ thống

 
Hình 3.3.1 Sơ đồ giao diện hệ thống

 
Hình 3.3.2 Sơ đồ quan hệ


 
 
Hình 3.3.3 Sơ đồ ERD
Mô tả chi tiết các bảng dữ liệu
1.	Bảng TaiKhoan (Quản lý admin)
 STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_admin	INT	Khóa chính	Mã định danh admin
2	Ten_admin	VARCHAR(100)	NOT NULL	Tên của admin
3	Email	VARCHAR(100)	NOT NULL	Email đăng nhập
4	So_dien_thoai	VARCHAR(20)		Số điện thoại liên hệ
5	Quyen_han	VARCHAR(50)	NOT NULL	Phân quyền của admin
6	Ngay_tao	DATETIME	DEFAULT NOW()	Ngày tạo tài khoản
 


2.	Bảng LoaiSP (Phân loại sản phẩm)
 STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_loai_san_pham	INT	Khóa chính	Mã loại sản phẩm
2	Ten_loai_san_pham	VARCHAR(100)	NOT NULL	Tên loại sản phẩm
3	Mo_ta_loai_san_pham	TEXT		Mô tả về loại sản phẩm
4	Ngay_tao	DATETIME	DEFAULT NOW()	Ngày tạo loại sản phẩm
 
3.	Bảng SanPham (Thông tin sản phẩm)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_sanpham	INT	Khóa chính	Mã định danh sản phẩm
2	Ten_sanpham	VARCHAR(100)	NOT NULL	Tên sản phẩm
3	Mo_ta	TEXT		Mô tả chi tiết sản phẩm
4	Gia_ban	DECIMAL(12,2)	NOT NULL	Giá bán sản phẩm
5	So_luong_ton_kho	INT	DEFAULT 0	Số lượng sản phẩm còn trong kho
6	ID_loai_sanpham	INT	Khóa ngoại	Liên kết với bảng LoaiSP
7	Ngay_tao	DATETIME	DEFAULT NOW()	Ngày tạo sản phẩm
 

4.	Bảng KhachHang (Thông tin khách hàng)
 STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_khachhang	INT	Khóa chính	Mã định danh khách hàng
2	Ten_khachhang	VARCHAR(100)	NOT NULL	Tên khách hàng
3	Dia_chi_giao_hang	VARCHAR(255)		Địa chỉ giao hàng
4	So_dien_thoai	VARCHAR(20)	NOT NULL	Số điện thoại liên hệ
5	Email	VARCHAR(100)		Email khách hàng
6	Ngay_dang_ky	DATETIME	DEFAULT NOW()	Ngày đăng ký tài khoản
 
5.	Bảng DonHang (Thông tin đơn hàng)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_donhang	INT	Khóa chính	Mã định danh đơn hàng
2	ID_khachhang	INT	Khóa ngoại	Liên kết với bảng KhachHang
3	Ngay_tao_donhang	DATETIME	DEFAULT NOW()	Ngày tạo đơn hàng
4	Trang_thai_donhang	VARCHAR(50)	NOT NULL	Trạng thái đơn hàng (Mới, Đang xử lý, Đang giao, Đã giao, Hủy)
5	Tong_gia_tri	DECIMAL(15,2)	NOT NULL	Tổng giá trị đơn hàng
6	ID_thanhtoan	INT	Khóa ngoại	Liên kết với bảng HinhThucThanhToan


6.	Bảng ChiTietDonHang (Chi tiết đơn hàng)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_chitiet_donhang	INT	Khóa chính	Mã định danh chi tiết đơn hàng
2	ID_donhang	INT	Khóa ngoại	Liên kết với bảng DonHang
3	ID_sanpham	INT	Khóa ngoại	Liên kết với bảng SanPham
4	So_luong_sanpham	INT	NOT NULL	Số lượng sản phẩm đặt mua
5	Gia_ban_sanpham	DECIMAL(12,2)	NOT NULL	Giá bán sản phẩm tại thời điểm đặt
6	Tong_gia	DECIMAL(15,2)	NOT NULL	Tổng giá (Số lượng × Giá bán)
 
7.	Bảng HinhThucThanhToan (Quản lý thanh toán)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_thanhtoan	INT	Khóa chính	Mã định danh thanh toán
2	Phuong_thuc_thanhtoan	VARCHAR(50)	NOT NULL	Phương thức thanh toán (Tiền mặt, Chuyển khoản, Thẻ tín dụng)
3	Trang_thai_thanhtoan	VARCHAR(50)	NOT NULL	Trạng thái thanh toán (Chưa thanh toán, Đã thanh toán, Hoàn tiền)
4	So_tien_thanhtoan	DECIMAL(15,2)	NOT NULL	Số tiền thanh toán
5	Ngay_thanhtoan	DATETIME		Ngày thực hiện thanh toán
 
8.	Bảng DanhGia (Đánh giá sản phẩm)
STT	Tên cột	Kiểu dữ liệu	Ràng buộc	Mô tả
1	ID_danhgia	INT	Khóa chính	Mã định danh đánh giá
2	ID_sanpham	INT	Khóa ngoại	Liên kết với bảng SanPham
3	ID_khachhang	INT	Khóa ngoại	Liên kết với bảng KhachHang
4	Xep_hang	INT	NOT NULL	Điểm đánh giá (1-5 sao)
5	Noi_dung_binh_luan	TEXT		Nội dung bình luận đánh giá
6	Ngay_dang	DATETIME	DEFAULT NOW()	Ngày đăng đánh giá
 
 

 
CHƯƠNG 4: HIỆN THỰC HỆ THỐNG
1.	Kiến trúc hệ thống
Hệ thống được thiết kế theo kiến trúc Client-Server, trong đó:
Client:
­	Là trình duyệt web của người dùng (Google Chrome, Firefox, Microsoft Edge).
­	Được sử dụng để gửi yêu cầu (request) và nhận dữ liệu (response) từ server.
­	Các giao diện được phát triển bằng HTML, CSS, JavaScript nhằm đảm bảo thân thiện và dễ sử dụng.
Server:
Được xây dựng với sự hỗ trợ của XAMPP, một phần mềm tích hợp sẵn các công cụ cần thiết:
­	Apache: Là máy chủ web xử lý các yêu cầu HTTP từ client.
­	MySQL: Là hệ quản trị cơ sở dữ liệu dùng để lưu trữ thông tin sản phẩm, khách hàng, đơn hàng.
­	PHP: Là ngôn ngữ lập trình phía server để xử lý logic và tương tác với cơ sở dữ liệu.
Server xử lý các yêu cầu từ client và trả về dữ liệu thích hợp, chẳng hạn như danh sách sản phẩm, chi tiết sản phẩm hoặc xác nhận đặt hàng.
 
CHƯƠNG 5: TỔNG KẾT
1.	Kết quả đạt được
Dự án thiết kế và phát triển hệ thống website bán đồ chơi đã hoàn thành với các kết quả chính sau:
Hoàn thiện các chức năng cốt lõi:
­	Hệ thống cho phép người dùng đăng ký, đăng nhập một cách bảo mật.
­	Khách hàng có thể duyệt danh mục sản phẩm, thêm sản phẩm vào giỏ hàng và thực hiện thanh toán.
­	Tích hợp tính năng tìm kiếm, giúp người dùng dễ dàng tìm thấy sản phẩm mong muốn.
­	Admin có thể quản lý sản phẩm, cập nhật thông tin và theo dõi đơn hàng.
Thiết kế giao diện:
­	Giao diện thân thiện với người dùng, hiển thị thông tin sản phẩm rõ ràng.
­	Tương thích trên các thiết bị khác nhau, bao gồm máy tính và thiết bị di động.
Xây dựng cơ sở dữ liệu tối ưu:
­	Cơ sở dữ liệu được thiết kế chặt chẽ với các bảng lưu trữ thông tin khách hàng, sản phẩm, đơn hàng và chi tiết đơn hàng.
­	Các truy vấn cơ sở dữ liệu đảm bảo tốc độ xử lý nhanh và tính toàn vẹn dữ liệu.
Ứng dụng công nghệ hiện đại:
­	Sử dụng XAMPP để triển khai môi trường phát triển và thử nghiệm.
­	Áp dụng các công nghệ như PHP, MySQL, HTML, CSS và JavaScript để xây dựng website.

2.	Hạn chế và kinh nghiệm
Hạn chế:
­	Chức năng bảo mật còn cơ bản:
Hệ thống hiện tại chỉ dừng ở mức sử dụng password_hash, chưa triển khai đầy đủ các phương thức bảo mật cao cấp như SSL cho giao tiếp an toàn.
­	Chưa tích hợp cổng thanh toán trực tuyến:
Hệ thống hiện mới hỗ trợ các phương thức thanh toán cơ bản, chưa kết nối với các cổng thanh toán thực tế như MoMo, PayPal.
­	Giao diện còn đơn giản:
Bố cục trang web chưa được đẹp
Thiết kế giao diện còn hạn chế về thẩm mỹ, cần cải thiện để hấp dẫn hơn với người dùng.
­	Chưa kiểm thử nâng cao:
Kiểm thử mới dừng lại ở mức chức năng cơ bản (Functional Testing), chưa thực hiện kiểm thử hiệu năng (Performance Testing) trên quy mô lớn.
Kinh nghiệm rút ra:
­	Cần học cách trình bày bố cục đẹp hơn
­	Học cách bảo mật chặt chẽ hơn
­	Nâng cao việc kiểm soát thời gian và làm việc nhóm
­	Cần học thêm nhiều kiến thức về thiết kế web

 
TÀI LIỆU THAM KHẢO

[1]. MYKINGDOM - VƯƠNG QUỐC ĐỒ CHƠI
[2]. Cách sử dụng xampp thành thục từ A-Z
[3]. https://www.fahasa.com/
…

