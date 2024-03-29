# CTDL & GT - Đồ án Quản Lý Thư Viện - KHÓA 2021 CNTT - ĐPT

## Thư viện: Ta tổ chức các danh sách sau:

-   `Đầu sách`: danh sách tuyến tính là 1 mảng con trỏ (ISBN , Tên sách, Số trang, Tác giả, năm xuất bản, thể loại, con trỏ dms): con trỏ sẽ trỏ đến các sách thuộc đầu sách tương ứng. Danh sách đầu sách luôn tăng dần theo tên sách.
-   `Danh mục sách` : danh sách liên kết đơn( Mã sách, trạng thái, vị trí ). Mỗi cuốn sách chỉ có 1 mã duy nhất; trạng thái của sách bao gồm: 0: cho mượn được, 1: đã có độc giả mượn, 2: sách đã thanh lý .
-   `Danh sách thẻ độc giả` : cây nhị phân tìm kiếm cân bằng (MATHE (số nguyên ngẫu nhiên tự động), Ho, Ten, Phai, trạng thái của thẻ, con trỏ): con trỏ sẽ trỏ đến danh sách các cuốn sách đã và đang mượn.
-   `Danh sách MUONTRA` : danh sách liên kết kép ( MASACH, NgayMuon, NgayTra, trạng thái): trạng thái =0 là sách đang mượn (chưa trả), =1 là đã trả, =2 : làm mất sách

## Chương trình có các chức năng sau:

-   a. Nhập thẻ độc giả: thêm / xóa / hiệu chỉnh thông tin thẻ độc giả. Mã thẻ độc giả được chương trình tự động lấy ngẫu nhiên và không trùng với các mã thẻ độc giả cũ; Phái chỉ nhận ‘Nam’ hoặc ‘Nữ’; trạng thái thẻ = 0 khi thẻ bị khóa, trạng thái thẻ = 1 khi thẻ đang hoạt động (được quyền mượn sách).
-   b. In danh sách độc giả : in ra màn hình theo thứ tự tên+họ tăng dần hoặc theo thứ tự mã độc giả tăng dần theo yêu cầu của thủ thư.
-   c. Nhập thông tin đầu sách và đánh mã sách tự động. Chương trình cho phép xóa 1 mã sách nếu mã sách này chưa cho độc giả mượn;
-   d. In danh sách các đầu sách trong thư viện theo từng thể loại, trong từng thể loại thì in theo thứ tự tên sách tăng dần.
-   e. Tìm thông tin sách dựa vào tên sách : in ra các thông tin mã ISBN, tên sách, tác giả, năm xuất bản, thể loại, các mã sách , trạng thái mã sách trong thư viện.
-   f. Mượn sách : nhập vào mã thẻ độc giả, chương trình sẽ liệt kê các sách mà độc giả đang mượn. Mỗi độc giả chỉ được mượn tối đa 3 cuốn, không cho mượn khi giữ 1 sách quá hạn (7 ngày) hoặc nếu các sách mượn thuộc cùng 1 đầu sách.
-   g. Trả sách
-   h. Liệt kê danh sách các mã sách, tên sách mà 1 độc giả có số thẻ X đang mượn
-   i. In danh sách độc giả mượn sách quá hạn theo thứ tự thời gian quá hạn giảm dần. Kết xuất :
    Mathe Ho tên Masach Tên sách Ngày mượn Số ngày quá hạn
-   j. In 10 đầu sách có số lượt mượn nhiều nhất.

## Cài đặt

Đồ án sử dụng thư viện giao diện winbgim.h, chạy trên IDE DevC++.

1. Cài đặt thư viện winbgim. [Xem hướng dẫn cài đặt tại đây](https://cachhoc.net/2013/10/03/cc-do-hoa-trong-dev-c/)
2. Tải về và giải nén source code.
3. Mở file `templeslibra.dev` bằng DevC++ và run project.

## Một số hình ảnh

![alt text](https://github.com/nhoczui3110/Library-Management/blob/main/pictures/demo-dausach1.png "Đầu sách")

![alt text](https://github.com/nhoczui3110/Library-Management/blob/main/pictures/demo-dausach2.png "Sách")

![alt text](https://github.com/nhoczui3110/Library-Management/blob/main/pictures/demo-dausach3.png "Hiệu chỉnh đầu sách")

![alt text](https://github.com/nhoczui3110/Library-Management/blob/main/pictures/demo-dausach4.png "Top 10 đầu sách")

![alt text](https://github.com/nhoczui3110/Library-Management/blob/main/pictures/demo-docgia1.png "Đọc giả")

![alt text](https://github.com/nhoczui3110/Library-Management/blob/main/pictures/demo-docgia2.png "Mượn trả")

![alt text](https://github.com/nhoczui3110/Library-Management/blob/main/pictures/demo-docgia3.png "Mượn trả")

![alt text](https://github.com/nhoczui3110/Library-Management/blob/main/pictures/demo-quahan.png "Danh sách quá hạn")
