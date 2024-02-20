# KTPM_UET
- Họ và tên: Trương Gia Ngọc. 
- MSV: 21020369

# Lý thuyết
## 1. Docker, docker-composer
- Docker là một nền tảng phần mềm hỗ trợ nhanh chóng việc triển khai một chương trình. Đóng gói các thành phần ở mức hệ điều hành như thư viện, công cụ hệ thống,... trong *container*, Docker cung cấp tất cả các thành phần cần thiết cho việc chạy một phần mềm. Sử dụng container cho phép quá trình thiết lập môi trường dễ dàng và thuận tiện hơn:  
  - Dễ ứng dụng.
  - Tốc độ nhanh.
  - Khả năng mở rộng.
- *Docker compose*: công cụ hỗ trợ việc định nghĩa và chạy các chương trình multi-container, là thành phần quan trọng trong quá trình phát triển phần mềm liên tục và hiệu quả. 
## 2.Linux, Unix, BSD hay *nix. Phân loại macOS
- **Unix**: là một hệ điều hành và là sản phẩm của một dự án bắt đầu từ năm 1969 với sự dẫn dắt của Ken Thompson và Dennis Ritchie trong phòng thí nghiệm của AT&T. Từ những năm thập niên 70, Unix được chia sẻ với các tổ chức thương mại và giáo dục, từ đó tạo nên các phiên bản khác, trong đó có BSD.
- **BSD (Berkeley Software Distribution)**: một trong các phiên bản của Unix của Computer Systems Research Group, đại học California, Berkeley. Được xây dựng trên code base và design của Unix. Một trong các hệ điều hành nguồn đóng phát triển từ BSD nổi tiếng là macOS.
- **Linux (GNU/Linux)**: hệ điều hành với nhân (kernel) Linux với các chương trình phần mềm của GNU. Việc config nhân cùng với quyết định các phần mềm được sử dụng có thể tùy biến, từ đó tạo ra các bản phân phối như Ubuntu, Debian, CentOS, Fedora,...
- ***nix**: *nix hay Unix-like là một khái niệm để chỉ các hệ điều hành được thiết kế vận hành tương tự như hệ điều hành Unix.
- Phân loại macOS: macOS là một hệ điều hành được phát triển dựa trên BSD. Đồng thời macOS cũng đạt chuẩn SUS (Single UNIX Specification). Dựa vào đó, macOS là một hệ điều hành Unix-like.
## 3. Alpine vs Ubuntu
- **Alpine**: Một bản phân phối Linux tập trung hướng đến sự nhỏ gọn, đơn giản và bảo mật
  - Nhỏ: Alpine được tạo ra với musl libc và busybox. Một container nặng không quá 8 MB và với bản cài đặt đơn giản nhất chỉ chiếm khoảng 130 MB.
  - Đơn giản: Tất cả những gì Alpine sử dụng là apk - bộ quản lý package của riêng Alpine, hệ thống khởi động OpenRC và setup hướng kịch bản, nhờ đó cung cấp cho người dùng một môi trường Linux đơn giản nhất.
  - Bảo mật: tất cả các chương trình được thực thi với vị trí ngẫu nhiên bởi kĩ thuật Position Independent Executables (PIE) - vị trí độc lập với thực thi và stack smash protection.
- **Ubuntu**: Bản phân phối Linux dựa trên Debian. Ubuntu có nhiều phiên bản hướng đến các mục tiêu sử dụng khác nhau, phổ biến nhất là cho máy cá nhân, server, điện toán đám mây, IoT và các hệ thống nhúng. Ubuntu dần trở nên phổ biến với người dùng phổ thông, bởi các lí do:
  - Thân thiện với người dùng: giao diện của Ubuntu được thiết kế dễ sử dụng, phù hợp với phần lớn người dùng.
  - Công cụ và phần mềm đa dạng: Ubuntu cung cấp lượng lớn các công cụ, package và tài liệu.
  - Cộng đồng lớn: Ubuntu có một cộng đồng người sử dụng lớn và được cập nhật thường xuyên nền những vấn đề thường được xử lí nhanh chóng.
## 4. VNC
- **VNC (Virtual Network Computing)**: hệ thống chia sẻ màn hình cross-platform sử dụng cho mục đích điều khiển một máy tính từ một máy khác ở xa. VNC họat động trên mô hình client/server với 2 thành phần:
  - Server: cài đặt trên máy cần điều khiến, truyền dữ liệu sao chép màn hình trên máy đến client.
  - Client hay VNC Viewer: cài đặt trên máy điều khiển, có thể gửi cả thông tin điều khiển chuột, bàn phím và cả thông tin chạm.
# Thực hành
