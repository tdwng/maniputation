# Lý thuyết về linux

## 1. File và cấu trúc file trong linux :

### a) File là gì? File được tổ chức như thế nào trong linux?

   Trong ngữ cảnh máy tính, file được hiểu là một tập hợp các thông tin, cho phép người dùng lưu trữ dữ liệu một cách đơn giản.

   Trong linux, file được tổ chức theo kiểu cây thư mục, nghĩa là tất cả các file, thư mục thuộc hệ thống đều nằm trong một nút gốc (root)

   Ta có thể dùng các lệnh trên terminal linux ví dụ như **ls**, **ls -l** ( nếu muốn cụ thể hơn) để liệt kê các file.

   Linux có nhiều loại file, bao gồm **file thường**, **thư mục**, **file thiết bị**, **file liên kết**, **socket file** và **pipe file**.

### b) Cấu trúc file '/' trong linux ( không biết diễn tả thế nào về cái thư mục gốc nên để tạm là '/' ):

   Thư mục gốc trong linux là **root**, thường được hiển thị với duy nhất kí tự **/**, từ thư mục này nó sẽ phân nhánh thành nhiều thư mục con khác, thường sẽ như hình minh họa  : ( Cùng là linux thì phần lớn sẽ không khác nhau mấy, dưới đây là của rasberry pi 4 model b, em xin phép không dùng ubuntu vm vì đợi nó start được thì em đã ăn xong 2 gói mì -.- )

   ![](image_1.png)

   Các thư mục con trong **/** thường bao gồm :

   **/bin** : Chứa các lệnh hệ thống cơ bản
   **/root** : Thư mục riêng của root user
   **/boot** : Chứa file khởi động hệ điều hành ( bootloader hoặc kernel )
   **/etc** : Chứa file cấu hình hệ thống 
   **/dev** : Chứa file thiết bị ( ví dụ ổ USB : **/dev/sdb**).
   **/home** : cd /home/< tên user >, đây là thư mục chứa user data 
   **/mnt** ( hoặc **/media** hoặc cả 2 :v ): Thư mục gắn kết ổ đĩa 
   **/lib** : Thư mục chứa thư viện hệ thống ( giống System32 trên Ưindows )
   **/opt** : Dùng để cài đặt các phần mềm ngoài ( VD cài chrome trên linux là cài phần mềm ngoài )
   **/proc** : Thông tin về tiến trình 
   **/sbin** : Chứa lệnh hệ thống cho **root**
   **/srv** : Dữ liệu cho web, server,...
   **/tmp** : Chứa file tạmp thời
   **/usr** : Chứa phần mềm, thư viện cho user
   **/var** : Chứa cache data, log data,... ( nói chung là dữ liệu thay đổi thường xuyên )

   Trên hình còn có một số thư mục như **/lost+found**, **/sys**, các thư viện này phục vụ mục đích khác nhau, như **/lost+found** check lại thiết bị khi ăn crash, check lỗi tập tin ; **/sys** chứa thông tin phần cứng, giao tiếp kernel,... ( Đoạn này lấy từ ChatGPT )

   





   
