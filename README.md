# BTL_Phattrienungdungdidong

# MÔN HỌC: PHÁT TRIỂN ỨNG DỤNG TRÊN THIẾT BỊ DI ĐỘNG - TEE0419 BÀI TẬP LỚN:

1. Viết phần mềm trên công cụ Mit App inventor (tập trung vào quy trình tạo ra phần mềm) app có 3 screen:
+ about về bản thân+nút gọi sang 2 screen còn lại
+ giải 1 bài toán đơn giản
+ sử dụng webview: hiển thị 1 trang web có sẵn, hỗ trợ giao diện điện thoại mô tả: thanh công cụ có gì? kéo thả + thay đổi thuộc tính: làm ntn, để làm gì? block: mô tả bản chất việc kéo thả block ntn? ưu điểm gì so với viết code? nhược điểm? copy paste block ? (backpack)
2. Viết app sử dụng Android Studio
- Android manifest.xml => mô tả gì? app cần quyền để do-st: khai báo ntn? để làm gì?
- vòng đời của 1 ứng dụng android. code tự sinh sau khi tạo 1 project: có sẵn hàm onCreate: tại sao???
- Code: java language. app cần check xem có quyền để do-st? : code ntn? ý nghĩa? giao diện: (res/layout) mô tả bằng file XML + UI Design review
   + thuộc tính text, hoặc các thuộc tính khác: giá trị hardcode => lưu vào nới khác, tham chiếu tới nó: cú pháp của việc tham chiếu là gì? ưu điểm của việc tham chiếu này? OS hỗ trợ auto việc lấy giá trị tham chiếu theo LOCATION, LANGUAGE, THEME việc hỗ trợ auto này giúp app làm được điều gì?
  + đối tượng chứa: gộp các đối tượng con lại: cùng 1 quy luật sắp xếp để hiển thị các đối tượng con nằm kề nhau theo chiều dọc | hoặc ngang, gravity code tương tác với layout: vd hiển thị text mong muốn text hiển thị phù hợp với thiết lập LOCATION, LANGUAGE, THEME của người dùng thì làm ntn? (tránh hardcode) event (sự kiện) người dùng tác động vào app: CLICK vào button, click vào text,... với 1 sự kiện nào đó, muốn chạy 1 đoạn code để do-st thì LAYTOUT cần làm gì? CODE viết như nào (2 cách)
``` text
 trong app có các thư mục đặc biệt: Assets
 khi sử dụng Window Explorer để copy các files + folder vào trong Assets
 thì khi compiler: mọi file này đều đi theo app, nằm trong app
 trong app có thể truy cập được đến các file này
 cú pháp truy cập vào là gì?
 lợi ích của việc app có sẵn các files (offline cũng có)?
 ứng dụng: app hướng dẫn việc X
``` 
==> tạo app1 sử dụng cơ chế Dữ liệu chuẩn bị trước trong Assets format dữ liệu: tuỳ ý, nội dung tuỳ ý công cụ để hiển thị dữ liệu: tuỳ ý có cần phải tiền xử lý trước khi hiển thị ko: tuỳ ý. SV TỰ ĐẶT RA VẤN ĐỀ => TỰ GIẢI QUYẾT VẤN ĐỀ MÔ TẢ ĐƯỢC DỮ LIỆU CÓ ĐẶC THÙ GÌ DÙNG THUẬT TOÁN NÀO ĐỂ XỬ LÝ DỮ LIỆU (NẾU CẦN) DÙNG ĐỐI TƯỢNG NÀO ĐỂ HIỂN THỊ DỮ LIỆU. (ĐỘ SÁNG TẠO LÀ KO GIỚI HẠN)

APP2 (android studio): tạo app tương đương với Mit App inventor app có 3 activity

- activity1: about: about+nút gọi sang 2 activity còn lại

- activity2: giải toán đơn giản (tuỳ ý). mỗi khi giải xong bài toán: gọi api tại https://k58kmt.tdh.io.vn/api để gửi bài toán lên đó {app_by:mã số sv, input: {a:1,b:2,c:3,name:"hello tắc kè"},output:{ketluan:"vô nghiệm", abc:"xyz", nghiem:3.14}} nhận lại json: {ok:1, stt:1234}

- activity3: dùng web-view để truy cập từ 1 trang web https://k58kmt.tdh.io.vn?masv=mã sv của bạn ======================= vết để lại: mô tả quá trình làm bài tập ra file .md => upload github kèm hình ảnh minh hoạ quá trình làm.

print ra giấy đóng quyển, nộp bm.
# BÀI LÀM
1. Viết phần mềm trên công cụ Mit App inventor
   - Tạo Project
      +  Vào appinventor.mit.edu → Create Apps! → đăng nhập Google
      +   Click Projects → Start new project → đặt tên ví dụ baitapcuanguyenthilinh
- Tạo Screen1 (About bản thân)

- Kéo Label -> Đổi nội dung -> Bên phải: Properties -> Tìm: Text -> đổi thành thông tin cá nhân ( làm y hệt như vậy với 2 label còn lại)

- Tạo Button: Kéo: Button -> Text: giải toán ( button Web view cũng làm tương tự)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/748c359d-1cf0-453c-b7f5-c61ad93162ee" />

- Nút mở Screen2

THIẾT KẾ SCREEN 2 (GIẢI PHƯƠNG TRÌNH ax+b=0)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/da3798c8-b3b5-46bb-abc9-3d834cd14e07" />

Viết Block giải toán

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4d2b40be-f10a-49ea-93cd-de7aea0921ad" />

THIẾT KẾ SCREEN 3

- ở phần url sẽ để https://www.google.com , để test thử xem phần mit app có hoạt động không
- Kéo thêm 1 dòng chữ (Label) từ cột User Interface bên trái thả vào màn hình, đặt nó nằm phía trên hoặc phía dưới cái WebViewer đó. Thay đổi chữ hiển thị của nút bấm thành: "bài tập của xuân trang".

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/480a08d1-76a4-4205-be9f-15ed459aa795" />

- kết quả test - Nút bấm chứa tên vẫn nằm ở đó, còn ô phía dưới thì hiển thị trang Google! Điều này chứng tỏ app của bạn hoạt động

<img width="828" height="1792" alt="image" src="https://github.com/user-attachments/assets/2e28b26e-b1bc-41d3-af05-1940b821cd9c" />


