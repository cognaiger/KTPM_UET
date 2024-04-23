# KTPM_UET
- Họ và tên: Trương Gia Ngọc. 
- MSV: 21020369

# Lý thuyết
## 1. Docker, docker-composer
- Docker là một nền tảng cung cấp cách để building, deploying và running ứng dụng dễ dàng hơn bằng cách sử dụng các containers (trên nền tảng ảo hóa). Docker đóng gói ứng dụng và các dependencies của nó trong *container*. Các container này khác VMs ở chỗ là container sẽ dùng chung tầng OS và các tầng bên dưới với host machine chứ không có riêng OS như VMs. Sử dụng container cho phép quá trình thiết lập môi trường dễ dàng và thuận tiện hơn:  
  - Dễ ứng dụng: Docker rất dễ cho mọi người sử dụng từ lập trình viên, sys admin… nó tận dụng lợi thế của container để build, test nhanh chóng. Có thể đóng gói ứng dụng trên laptop của họ và chạy trên public cloud, private cloud… Câu thần chú là
    “Build once, run anywhere”.
  - Tốc độ nhanh: Docker container rất nhẹ và nhanh, bạn có thể tạo và chạy docker container trong vài giây.
  - Khả năng mở rộng: Bạn có thể chia nhỏ những chức năng của ứng dụng thành các container riêng lẻ.
- *Docker compose*: công cụ dùng để định nghĩa và run multi-container cho Docker application. Ta dùng docker compose khi ứng dụng của chúng ta có nhiều layer, mỗi layer sẽ được đặt trong một container để có thể quản lý môi trường tốt hơn và giảm
  sự phụ thuộc chồng chéo giữa các layer. Docker-compose cung cấp cho ta cách để quản lý multi-container application như quản lý một ứng dụng thống nhất
    ![image](https://github.com/cognaiger/KTPM_UET/assets/100193663/f4a09e9c-7dc9-44de-9cfb-30df3b4e104d)

## 2.Linux, Unix, BSD hay *nix. Phân loại macOS
- **Unix**: là một hệ điều hành và là sản phẩm của một dự án bắt đầu từ năm 1969 với sự dẫn dắt của Ken Thompson và Dennis Ritchie trong phòng thí nghiệm của AT&T. Từ những năm thập niên 70, Unix được chia sẻ với các tổ chức thương mại và giáo dục, từ đó tạo nên các phiên bản khác, trong đó có BSD.
- **BSD (Berkeley Software Distribution)**: một trong các phiên bản của Unix của Computer Systems Research Group, đại học California, Berkeley. Được xây dựng trên code base và design của Unix. Một trong các hệ điều hành nguồn đóng phát triển từ BSD nổi tiếng là macOS.
- **Linux (GNU/Linux)**: hệ điều hành với nhân (kernel) Linux với các chương trình phần mềm của GNU. Việc config nhân cùng với quyết định các phần mềm được sử dụng có thể tùy biến, từ đó tạo ra các bản phân phối như Ubuntu, Debian, CentOS, Fedora,...
- ***nix**: *nix hay Unix-like là một khái niệm để chỉ các hệ điều hành được thiết kế vận hành tương tự như hệ điều hành Unix.
- **macOS**: macOS là một hệ điều hành được phát triển dựa trên BSD. Đồng thời macOS cũng đạt chuẩn SUS (Single UNIX Specification). Dựa vào đó, macOS là một hệ điều hành Unix-like. macOS có các phiên bản như macOS Monterey, macOS Catalina, macOS
  Mojave, macOS High Sierra
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
- **VNC (Virtual Network Computing)**: hệ thống chia sẻ màn hình cross-platform sử dụng cho mục đích điều khiển một máy tính từ một máy khác ở xa. VNC họat động trên mô hình client/server với các thành phần:
  - Server: cài đặt trên máy cần điều khiến, truyền dữ liệu sao chép màn hình trên máy đến client.
  - Client hay VNC Viewer: cài đặt trên máy điều khiển, có thể gửi cả thông tin điều khiển chuột, bàn phím và cả thông tin chạm.
  - VNC Protocol: Giao thức VNC là một giao thức đơn giản cho việc truy cập từ xa vào giao diện đồ họa. Giao thức này đơn giản cho phép một máy chủ cập nhật khung hình hiển thị trên một viewer. Bởi vì nó hoạt động ở mức framebuffer, nó có thể áp
    dụng cho tất cả các hệ điều hành bao gồm X/Unix, Windows 3.1/95/NT và Macintosh. Giao thức này sẽ hoạt động trên bất kỳ đường truyền tin cậy nào như TCP/IP.
  
      ![image](https://github.com/cognaiger/KTPM_UET/assets/100193663/620df422-c3e7-41fb-b2b6-458a3bd728f6)

# Thực hành
