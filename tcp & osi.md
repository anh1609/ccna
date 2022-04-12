

## Giới thiệu  MÔ HÌNH THAM CHIẾU OSi

1. #### Mô hình tham chiếu

Ý nghĩa quan trọng nhất của mô hình OSI đó là tính tham chiếu. Mô hình OSI mô tả hoàn chỉnh quá trình truyền và gửi dữ liệu giữa 2 thiết bị mạng bất kỳ cũng như quá trình dữ liệu truyền đi từ ứng dụng người dùng này, tới các môi trường truyền dẫn và sang ứng dụng người dùng phía bên kia

2. #### Kiến trúc phân lớp

Mô hình OSI cố gắng phân chia và gộp các chức năng mạng có chức năng tương tự nhau thành các tầng. Mỗi tầng sẽ cung cấp dịch vụ cho tầng phía trên, và nhận dịch vụ từ tầng phía dưới. Mô hình OSI bao gồm 7 tầng và mỗi tầng đảm nhiệm những nhiệm vụ khác nhau trong toàn bộ quá trình truyền dữ liệu. Những lợi ích của việc tiếp cận theo kiến truc phân lớp

* Giảm độ phức tạp do cả quá trình truyền dẫn được chia nhỏ thành các phần nhỏ hơn
* Chuẩn hóa chức năng trên giao diện
* Cho phép các thành phần phần cứng và phần mềm tương tác với nhau
* Đơn giản hóa quá trình học tập và trao đổi kiến thức

Kiến trúc phân lớp là một cách tiếp cận đơn giản nhưng vô cùng hiệu quả, linh hoạt. Bất kỳ một giao thức hoặc công nghệ mới được phát triển không làm phá vỡ cấu trúc của mô hình, điều này thúc đẩy việc nghiên cứu và linh động trong việc cung cấp các giải pháp. Chẳng hạn việc chuyển sang sử dụng địa chỉ Ipv6 từ IPv4 không đồng nghĩa với việc phải thay đổi các ứng dụng hoặc các cơ chế truyền dữ liệu trên một môi trường truyền dẫn, hoặc đơn giản, card mạng NIC trên PC không cần quan tâm tới nội dung trang web được truy cập, ngược lại, trình duyệt web không cần biết công nghệ chạy trên card mạng NIC có phải là Ethernet hay không 

3. #### Các tầng OSI

7 tầng OSI bao gồm:

* Tầng 7 – Tầng ứng dụng: Thông qua các giao thức, cung cấp giao diện giữa phần mềm với các ứng dụng người dùng (chẳng hạn email, truyền file, ứng dụng đầu cuối…) có mong muốn trao đổi dữ liệu trên nhiều thiết bị
* Tầng 6 – Tầng trình diễn: Làm nhiệm vụ định nghĩa và trao đổi các định dạng dữ liệu, chẳng hạn ASCII, jpeg, wmv…Đảm bảo việc thay đổi trên một tầng không ảnh hưởng đến các tầng khác, hỗ trợ việc phát triển trên từng tầng nhưng không phải viết lại toàn bộ mô hình
Đơn giản hóa quá trình học tập và trao đổi kiến thức

* Tầng 5 – Tầng phiên: Làm nhiệm vụ thiết lập, điều khiển và ngắt một phiên kết nối ứng dụng

* Tầng 4 – Tầng chuyển vận: Làm nhiệm vụ phân mảnh các dòng dữ liệu thành các mảnh nhỏ gọi là segment và ngược lại. Cung cấp các dịch vụ để đảm bảo việc trao đổi giữa các ứng dụng khác nhau được thông suốt, các dịch vụ điều khiển luồng, sửa lỗi và truyền thông tin cậy

* Tầng 3 – Tầng mạng: Làm nhiệm vụ đánh địa chỉ logic, cấu trúc địa chỉ Internet và định tuyến liên mạng

* Tầng 2 – Tầng liên kết dữ liệu: Làm nhiệm vụ điều khiển quá trình gửi nhận và điều khiển truy cập môi trường truyền
* Tầng 1 – Tầng Vật lý: Làm nhiệm vụ mã hóa dữ liệu các bit nhị phân sau đó chuyển thành tín hiệu để truyền trong môi trường

Dựa trên chức năng và cấu trúc tầng chúng ta có thể chia thành 2 nhóm: Các tầng nửa trên (Tầng 4,5,6,7) tập trung vào các chức năng ứng dụng, các tầng nửa dưới (Tầng 1,2,3,4) tập trung vào các chức năng truyền dẫn dữ liệu 

Phân loại một vài giao thưc và thiết bị tiêu biểu dựa trên mô hình OSI

| Tầng      |Giao thức và các chuẩn       |Thiết bị    |
|:----- |:-----  |:-----   |
|5- 7 : Tầng Ứng dung, trình diễn, phiên            |Telnet, HTTP, FTP, DNS, SMTP, POP3, VoIP, SNMP               | Tưởng lửa, IDS |
| 4 : Tầng chuyển vận | TCP, UDP          |           |
|3 : Tầng Mạng |   IP|   Router |
|2 : Tầng Liên kết dữ liệu |Ethernet, HDLC, Frame-relay, PPP|Switch, Wireless AP, DSL modem |
|1 : Tầng Vật lý|Ethernet, RJ-45, V.35|Hub, bộ lặp|

4. #### So sánh với mô hình TCP/IP
5. #### Kỹ thuật đóng gói (encapsulation)

