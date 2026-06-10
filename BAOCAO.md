# BaiTapLon_PhatTrienUngDUngTrenThietBiDiDong
# Nguyễn Lam Sơn_K225480106076
## MÔN HỌC: PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419
# BÀI TẬP LỚN:
# 1. Viết phần mềm trên công cụ Mit App inventor <br>
   (tập trung vào quy trình tạo ra phần mềm) <br>
   app có 3 screen: <br>
   + about về bản thân+nút gọi sang 2 screen còn lại <br>
   + giải 1 bài toán đơn giản <br>
   + sử dụng webview: hiển thị 1 trang web có sẵn, hỗ trợ giao diện điện thoại <br>
   mô tả: thanh công cụ có gì? kéo thả + thay đổi thuộc tính: làm ntn, để làm gì? <br>
          block: mô tả bản chất việc kéo thả block ntn? <br>
                 ưu điểm gì so với viết code? nhược điểm? <br>
                 copy paste block ? (backpack) <br>
# 2. Viết app sử dụng Android Studio <br>
   + Android manifest.xml  => mô tả gì? app cần quyền để do-st: khai báo ntn? để làm gì? <br>
   + vòng đời của 1 ứng dụng android. <br>
     code tự sinh sau khi tạo 1 project: có sẵn hàm onCreate: tại sao??? <br>
   + Code: java language. <br>
     app cần check xem có quyền để do-st? : code ntn? ý nghĩa? <br>
     giao diện: (res/layout) mô tả bằng file XML + UI Design review <br>
        + thuộc tính text, hoặc các thuộc tính khác: giá trị hardcode => lưu vào nới khác, tham chiếu tới nó: <br>
          cú pháp của việc tham chiếu là gì? <br>
          ưu điểm của việc tham chiếu này? <br>
          OS hỗ trợ auto việc lấy giá trị tham chiếu theo LOCATION, LANGUAGE, THEME <br>
          việc hỗ trợ auto này giúp app làm được điều gì?	<br>
        + đối tượng chứa: gộp các đối tượng con lại: cùng 1 quy luật sắp xếp để hiển thị <br>
          các đối tượng con nằm kề nhau theo chiều dọc | hoặc ngang, gravity <br>
     code tương tác với layout: vd hiển thị text <br>
          mong muốn text hiển thị phù hợp với thiết lập LOCATION, LANGUAGE, THEME của người dùng <br>
          thì làm ntn? (tránh hardcode) <br>
     event (sự kiện) người dùng tác động vào app: CLICK vào button, click vào text,... <br>
          với 1 sự kiện nào đó, muốn chạy 1 đoạn code để do-st <br>
          thì LAYTOUT cần làm gì? <br>
              CODE viết như nào (2 cách) <br>
---------------------------
     trong app có các thư mục đặc biệt: Assets
     khi sử dụng Window Explorer để copy các files + folder vào trong Assets
     thì khi compiler: mọi file này đều đi theo app, nằm trong app
     trong app có thể truy cập được đến các file này
     cú pháp truy cập vào là gì?
     lợi ích của việc app có sẵn các files (offline cũng có)?
     ứng dụng: app hướng dẫn việc X

==> tạo app1 sử dụng cơ chế Dữ liệu chuẩn bị trước trong Assets <br>
       -  format dữ liệu: tuỳ ý, nội dung tuỳ ý <br>
       -  công cụ để hiển thị dữ liệu: tuỳ ý <br>
       - có cần phải tiền xử lý trước khi hiển thị ko: tuỳ ý. <br>
       - SV TỰ ĐẶT RA VẤN ĐỀ => TỰ GIẢI QUYẾT VẤN ĐỀ <br>
       - MÔ TẢ ĐƯỢC DỮ LIỆU CÓ ĐẶC THÙ GÌ <br>
                   1. DÙNG THUẬT TOÁN NÀO ĐỂ XỬ LÝ DỮ LIỆU (NẾU CẦN) <br>
                   2. DÙNG ĐỐI TƯỢNG NÀO ĐỂ HIỂN THỊ DỮ LIỆU. <br>
                   3. (ĐỘ SÁNG TẠO LÀ KO GIỚI HẠN) <br>
------------------------
APP2 (android studio):  tạo app tương đương với Mit App inventor <br>
  app có 3 activity <br>
  + activity1: about: about+nút gọi sang 2 activity còn lại <br>
  + activity2: giải toán đơn giản (tuỳ ý). mỗi khi giải xong bài toán: gọi api tại https://k58kmt.tdh.io.vn/api <br>
    để gửi bài toán lên đó <br>
    {app_by:mã số sv, input: {a:1,b:2,c:3,name:"hello tắc kè"},output:{ketluan:"vô nghiệm", abc:"xyz", nghiem:3.14}} <br>
    nhận lại json: {ok:1, stt:1234} <br>
  + activity3: <br>
    dùng web-view để truy cập từ <br>
    1 trang web https://k58kmt.tdh.io.vn?masv=mã sv của bạn <br>
======================= <br>
    vết để lại: mô tả quá trình làm bài tập ra file .md => upload github <br>
    kèm hình ảnh minh hoạ quá trình làm. <br>

    print ra giấy đóng quyển, nộp bm. <br>
# BÀI LÀM:
# PHẦN 1
## 1. LÀM APP TRÊN MIT APP INVENTOR
# Địa chỉ công cụ: http://ai2.appinventor.mit.edu/ (Đăng nhập bằng tài khoản Google).
## Cách thực hiện: <br>
Tạo App: Click Projects -> Start new project -> Đặt tên: BaiTapLon_App1. <br> 
Tạo 3 Màn hình (Screen): Góc trên bên phải có nút Add Screen. Bạn tạo thêm Screen2 và Screen3. <br>
Thiết kế Giao diện (Tab Designer): <br>
Screen1 (About): Cột Palette (bên trái), kéo Image, Label (ghi thông tin của bạn) và 2 Button vào màn hình giữa (Viewer). Sang cột Properties (bên phải) đổi tên Button thành "Chuyển Screen 2" và "Chuyển Screen 3". <br>
Screen2 (Toán): Kéo 2 TextBox (để nhập a, b), 1 Button (Giải), 1 Label (Hiển thị kết quả). <br>
Screen3 (Web): Góc trái tìm mục User Interface, kéo linh kiện WebViewer vào. Nhìn sang phải cột Properties, ô HomeUrl dán link: https://m.dantri.com.vn. <br>
Viết logic (Tab Blocks ở góc phải trên cùng): <br>
Ở Screen1: Click vào Button1 bên menu trái, kéo khối when Button1.Click do. Vào mục Control, kéo khối open another screen screenName và ghép vào. Gõ "Screen2". Làm tương tự cho Button 2 chuyển sang "Screen3". <br>
Ở Screen2: Dùng khối toán học (Math) để lập trình cộng/trừ 2 TextBox hiển thị ra Label. <br>
# Thực Hành:
1 Tạo Projects đătj tên là baitaplon
# <img width="1917" height="926" alt="image" src="https://github.com/user-attachments/assets/ceb8198d-43e4-4321-9dd8-de42f0a1d596" />
2 Add Screen.tạo thêm Screen2 và Screen3.
# <img width="632" height="237" alt="image" src="https://github.com/user-attachments/assets/f614b9a4-f86e-42a5-ad6f-b8485bf6dbb3" />
3 Thiết kế Giao diện
## screen1: 
# <img width="1918" height="1025" alt="image" src="https://github.com/user-attachments/assets/2e2021d1-4d63-4b09-a96c-77036b8a53c1" />
## screen2:
# <img width="1918" height="1027" alt="image" src="https://github.com/user-attachments/assets/41f1b3e9-717d-42a9-84f9-91b70b706937" />
## csreen3:
# <img width="1918" height="1023" alt="image" src="https://github.com/user-attachments/assets/c0f41239-df50-42e0-a66d-e7ff998880c3" />
# 2. VIẾT LOGIC (TAB BLOCKS - GÓC TRÊN CÙNG BÊN PHẢI)
Bấm vào nút Blocks ở góc trên cùng bên phải để chuyển từ giao diện thiết kế sang giao diện ghép khối lệnh. <br>
## 1. Viết logic cho Screen1 (Chuyển màn hình) <br>
Viết logic cho Screen1 (Chuyển màn hình) <br>
(Đảm bảo bạn đang chọn Screen1 ở góc trái) <br>
## Bước 1: Ở menu bên trái, bấm vào chữ Btn_Toan. 
Nó sẽ hiện ra một loạt khối lệnh màu vàng. Bạn lấy con chuột kéo khối when Btn_Toan.Click do thả ra màn hình trống ở giữa. <br>
## Bước 2: Ở menu bên trái, bấm vào danh mục Control (màu vàng đậm hệ thống). 
Kéo khối open another screen screenName gắn vào bên trong cái miệng chữ do của khối <br>
## Bước 3: Ở menu bên trái, bấm vào danh mục Text (màu hồng). 
Kéo khối chuỗi rỗng có dấu ngoặc kép "" gắn vào vị trí screenName. <br>
Sau đó click chuột vào trong dấu <br>
ngoặc kép đó và gõ đúng chữ: Screen2 (chú ý viết hoa chữ S, viết liền không dấu). <br>
## Làm tương tự cho nút Web: Kéo khối when Btn_Web.Click do -> gắn khối open another screen screenName -> gắn khối "" và gõ vào chữ Screen3. <br>
# <img width="840" height="468" alt="image" src="https://github.com/user-attachments/assets/572094b0-a543-40e8-a3f8-e8f876b8785c" />
## 2. Viết logic cho Screen2 (Lập trình phép toán cộng a + b)
Viết logic cho Screen2 
(Lập trình phép toán cộng $a + b$)
(Bấm chọn chuyển sang màn hình Screen2 ở menu góc trên bên trái, sau đó chọn Tab Blocks)
## Bước 1:Ở menu bên trái, bấm vào chữ Btn_TinhTong. 
Kéo khối when Btn_TinhTong.Click do thả ra màn hình trống.
## Bước 2: Ở menu bên trái, bấm vào chữ Lbl_KetQua.
Kéo khối set Lbl_KetQua.Text to gắn vào bên trong miệng chữ do.
## Bước 3: Ở menu bên trái, bấm vào danh mục Math (màu xanh dương).
Tìm và kéo khối phép cộng có dấu cộng + (... + ...) gắn vào sau chữ to của khối bước 2.
## Bước 4: Ở menu bên trái, bấm vào chữ Txt_SoA.
Tìm khối lệnh tên là Txt_SoA.Text (màu xanh lá cây nhạt) kéo ra gắn vào ô trống thứ nhất của phép cộng +.
## Bước 5: Ở menu bên trái, bấm vào chữ Txt_SoB. 
Tìm khối lệnh tên là Txt_SoB.Text kéo ra gắn vào ô trống thứ hai còn lại của phép cộng +.
# <img width="1918" height="947" alt="image" src="https://github.com/user-attachments/assets/2c39d7f8-141f-4ef8-a6b0-f3f5cd555241" />
# NỘI DUNG LÝ THUYẾT VỀ LOGIC:
## Quy trình thiết kế giao diện ứng dụng (Tab Designer)
Ứng dụng được thiết kế gồm 3 màn hình (Screen) cụ thể như sau:

* **Screen1 (About Bản Thân):** - Sử dụng đối tượng `Image1` hiển thị ảnh đại diện cá nhân (`anh_the_nguyen_lam_son.jpg`).
  - Sử dụng các `Label1`, `Label2`, `Label3` để hiển thị thông tin tĩnh bao gồm: "Họ và tên: Nguyễn Lam Sơn", "MSSV: 20261234", "Lớp: K58KMT".
  - Sử dụng 2 nút bấm `Btn_Toan` và `Btn_Web` định dạng chữ hiển thị để người dùng click chuyển trang.
  # <img width="1918" height="1025" alt="image" src="https://github.com/user-attachments/assets/2e2021d1-4d63-4b09-a96c-77036b8a53c1" />

* **Screen2 (Bài toán đơn giản):**
  - Thiết kế bài toán tính tổng hai số nhập vào từ bàn phím.
  - Sử dụng `Txt_SoA` và `Txt_SoB` cấu hình thuộc tính `NumbersOnly = True` để bắt buộc nhập số.
  - Sử dụng `Btn_TinhTong` để kích hoạt sự kiện xử lý.
  - Sử dụng `Lbl_KetQua` đổi màu chữ sang màu Đỏ để hiển thị kết quả đầu ra.
# <img width="1918" height="1027" alt="image" src="https://github.com/user-attachments/assets/41f1b3e9-717d-42a9-84f9-91b70b706937" />

* **Screen3 (WebView hiển thị trang báo):**
  - Kéo linh kiện `WebViewer1` chiếm toàn màn hình.
  - Thay đổi thuộc tính `HomeUrl` trỏ thẳng tới địa chỉ: `https://m.dantri.com.vn` để tự động tải giao diện báo điện tử hỗ trợ mobile.
# <img width="1918" height="1023" alt="image" src="https://github.com/user-attachments/assets/c0f41239-df50-42e0-a66d-e7ff998880c3" />

## 2. Mô tả các thành phần hệ thống và Bản chất lập trình Block
* **Thanh công cụ quản lý:**
  - *Palette:* Nơi chứa toàn bộ kho linh kiện gốc của hệ thống Android.
  - *Viewer:* Màn hình giả lập hiển thị giúp sắp xếp bố cục linh kiện bằng mắt thường.
  - *Components:* Cây quản lý phân cấp, giúp quản lý và đổi tên định danh ID đối tượng (ví dụ: đổi từ Button1 thành Btn_Toan).
  - *Properties:* Bản tùy chỉnh chi tiết thông số linh kiện (màu sắc, kích cỡ chữ, kích thước dài rộng).

* **Bản chất của việc kéo thả Block:**
  - Bản chất là lập trình trực quan hướng sự kiện. Thay vì phải gõ từng dòng mã lệnh, người lập trình ghép nối các khối logic toán học, văn bản và điều khiển có sẵn lại với nhau. Hệ thống thiết kế các rãnh khớp nối thông minh, nếu ghép sai kiểu dữ liệu (ví dụ ghép chữ vào phép toán cộng), khối lệnh sẽ không khít nhau, từ đó triệt tiêu hoàn toàn lỗi cú pháp (Syntax Error) như thiếu dấu `;` hay dấu `{}` trong code truyền thống.
  - *Ưu điểm:* Dễ tiếp cận, trực quan, tốc độ xây dựng luồng ứng dụng cực nhanh.
  - *Nhược điểm:* Khi logic phình to, giao diện kéo thả blocks cực kỳ rối mắt, khó quản lý mã nguồn và hạn chế can thiệp sâu vào các tính năng phần cứng nâng cao của hệ điều hành.

* **Tính năng Backpack (Cái Balo):**
  - Nằm ở góc trên bên phải màn hình Blocks. Đây là bộ nhớ đệm dùng để lưu trữ tạm thời các khối logic phức tạp. Khi muốn nhân bản đoạn code chuyển màn hình từ Screen1 sang áp dụng cho các màn hình khác, ta chỉ cần kéo cụm block đó thả vào Backpack, sau đó sang màn hình mới mở Backpack ra kéo thả ngược lại. Đây chính là cơ chế Copy - Paste mã nguồn trực quan.
# <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/61306bcc-bd17-4508-bce9-3de06c6ef09b" />
# PHẦN 2: ANDROID STUDIO - KIẾN THỨC NỀN TẢNG (LÝ THUYẾT & CHUẨN BỊ)
Mở Android Studio -> Chọn New Project -> Empty Views Activity
## 2.1 AndroidManifest.xml là gì?
- Nó là "giấy khai sinh" và là bảng cấu hình của ứng dụng. Mọi Activity bạn tạo ra, mọi quyền truy cập hệ thống đều phải khai báo ở đây.
- xin quyền dùng Internet (phục vụ cho tính năng WebView), gõ dòng lệnh này vào # <uses-permission android:name="android.permission.INTERNET" />
# <img width="1452" height="981" alt="image" src="https://github.com/user-attachments/assets/29c74ac0-3217-4b67-9690-b49291edc6f5" />
## 2.2 Vòng đời ứng dụng & File Code Java
- Ứng dụng Android viết bằng ngôn ngữ Java. Nó có một vòng đời trải qua nhiều trạng thái (mở app, ẩn xuống nền, tắt app). Hàm onCreate luôn có sẵn khi tạo project vì đây là bước đầu tiên trong vòng đời ứng dụng khi màn hình được tạo ra; nó chịu trách nhiệm khởi tạo các biến và liên kết giao diện người dùng. <br>
- Mở thư mục: MainActivity.java
- mọi code tương tác cơ bản ở giai đoạn đầu sẽ viết bên trong hàm này: onCreate
# <img width="1397" height="561" alt="image" src="https://github.com/user-attachments/assets/ebc30cd6-9b41-4797-bbe3-5e123964d438" />
## 2.3. Thiết kế giao diện (Layout) & Tránh Hardcode
- Giao diện được mô tả bằng file XML nằm trong thư mục res/layout. Để tránh hardcode (viết thẳng giá trị chết vào giao diện), bạn phải lưu các thuộc tính text vào một nơi khác rồi tham chiếu tới nó <br>
** Ưu điểm của việc này là hệ điều hành (OS) sẽ tự động lấy giá trị tham chiếu theo Location (Vị trí), Language (Ngôn ngữ), Theme (Chủ đề) của người dùng. Việc hỗ trợ auto này giúp app tự động chuyển đổi ngôn ngữ hoặc giao diện sáng/tối mà lập trình viên không cần viết thêm code <br>
- Mở file res/values/strings.xml: Thêm một dòng: <string name="loi_chao">Xin chào bạn</string> <br>
# <img width="822" height="341" alt="image" src="https://github.com/user-attachments/assets/70d11603-979f-4bbc-9171-9e9df6f75c0f" />
- Tiếp theo, mở file giao diện res/layout/activity_main.xml: Khi tạo một chữ hiển thị, thay vì viết android:text="Xin chào bạn" (đây là hardcode),viết cú pháp tham chiếu: android:text="@string/loi_chao" <br>
# <img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/a3b79edb-5e0d-4059-a82b-b89d1334b4c1" />


