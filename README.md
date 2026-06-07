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
# MÔ TẢ QUY TRÌNH TẠO PHẦN MỀM TRÊN MIT APP INVENTOR

## 1. Thanh công cụ trong MIT App Inventor

Trong quá trình xây dựng ứng dụng bằng MIT App Inventor, công cụ cung cấp nhiều khu vực hỗ trợ thiết kế và lập trình ứng dụng.

### 1.1 Palette

Palette là khu vực chứa các component dùng để xây dựng ứng dụng bằng phương pháp kéo thả.

Một số component thường sử dụng gồm:

* **Button**: dùng để tạo nút bấm
* **Label**: dùng để hiển thị văn bản
* **TextBox**: dùng để nhập dữ liệu từ người dùng
* **Image**: dùng để hiển thị hình ảnh
* **WebViewer**: dùng để hiển thị website trong ứng dụng
* **Layout**: dùng để bố trí giao diện

**Mục đích:**
Giúp người dùng lựa chọn component cần thiết để xây dựng giao diện ứng dụng.

---

### 1.2 Viewer

Viewer là khu vực mô phỏng màn hình điện thoại.

Người dùng thực hiện kéo thả component trực tiếp từ Palette vào Viewer để xây dựng giao diện.

**Mục đích:**
Cho phép xem trước giao diện ứng dụng trong quá trình thiết kế.

---

### 1.3 Components

Components là khu vực hiển thị danh sách toàn bộ thành phần đang tồn tại trong màn hình.

Ví dụ:

* Button1
* TextBox1
* Label1

**Mục đích:**
Giúp quản lý các component dễ dàng hơn trong quá trình thiết kế ứng dụng.

---

### 1.4 Properties

Properties là khu vực dùng để thay đổi thuộc tính của component.

Một số thuộc tính thường dùng:

* **Text**: nội dung hiển thị
* **Width / Height**: kích thước component
* **FontSize**: kích thước chữ
* **BackgroundColor**: màu nền
* **Visible**: hiển thị hoặc ẩn component

Ví dụ:

Khi tạo một Button, có thể chỉnh:

* Text = “Tính”
* Width = Fill Parent
* BackgroundColor = Blue

**Mục đích:**
Giúp thay đổi giao diện và hành vi của component theo nhu cầu sử dụng.

---

## 2. Kéo thả component và thay đổi thuộc tính

MIT App Inventor sử dụng phương pháp kéo thả component để tạo giao diện ứng dụng.

### Cách thực hiện

**Bước 1:**
Chọn component trong mục **Palette**.

**Bước 2:**
Kéo thả component vào khu vực **Viewer**.

**Bước 3:**
Chọn component vừa thêm và chỉnh thuộc tính trong **Properties**.

Ví dụ:

Kéo **Button** vào màn hình và chỉnh:

* Text = “Tính”
* Width = Fill Parent
* FontSize = 18

### Mục đích

* Giúp tạo giao diện nhanh chóng
* Không cần viết code giao diện thủ công
* Dễ chỉnh sửa trực tiếp khi thiết kế

---

## 3. Block trong MIT App Inventor

### Bản chất của Block

MIT App Inventor sử dụng phương pháp lập trình trực quan bằng block kéo thả.

Thay vì phải viết code bằng Java hoặc Kotlin, người dùng chỉ cần kéo các block logic và ghép nối lại với nhau để tạo chức năng cho ứng dụng.

Ví dụ:

Khi người dùng nhấn nút Button:

```text
when Button1.Click
```

thì ứng dụng sẽ thực hiện đoạn xử lý được nối phía dưới.

Trong bài tập này, block được sử dụng để giải phương trình bậc nhất:

```text
when Button1.Click
set Label2.Text to
((0 - TextBox2.Text) / TextBox1.Text)
```

Mục đích của block trên là tính nghiệm:

[
x=-\frac{b}{a}
]

sau đó hiển thị kết quả lên màn hình.

### Cách kéo thả block

**Bước 1:**
Chọn tab **Blocks**.

**Bước 2:**
Chọn component cần xử lý.

**Bước 3:**
Kéo block chức năng vào vùng làm việc.

**Bước 4:**
Ghép các block logic với nhau để hoàn thiện chức năng.

Ví dụ:

* block Click
* block tính toán
* block hiển thị kết quả

---

## 4. Ưu điểm của block so với viết code

### Ưu điểm

* Dễ học và dễ sử dụng
* Không cần nhớ cú pháp lập trình
* Hạn chế lỗi syntax
* Trực quan, dễ quan sát luồng xử lý
* Phù hợp với người mới học phát triển ứng dụng di động

---

## 5. Nhược điểm của block

### Nhược điểm

* Khi project lớn sẽ có nhiều block gây khó quản lý
* Khó tối ưu hiệu năng ứng dụng
* Ít linh hoạt hơn so với lập trình Java hoặc Kotlin
* Một số chức năng nâng cao khó triển khai

---

## 6. Copy và Paste block bằng Backpack

### Backpack là gì?

Backpack là công cụ dùng để lưu trữ và tái sử dụng block trong MIT App Inventor.

### Cách sử dụng

**Bước 1:**
Nhấn chuột phải vào block cần sao chép.

**Bước 2:**
Chọn:

```text
Add to Backpack
```

**Bước 3:**
Chuyển sang screen khác hoặc project khác.

**Bước 4:**
Mở Backpack và dán lại block.

### Mục đích

* Tiết kiệm thời gian lập trình
* Không cần tạo lại block nhiều lần
* Có thể tái sử dụng logic giữa các screen

### Ưu điểm của Backpack

* Giảm thời gian thiết kế
* Dễ dàng tái sử dụng block
* Giảm lỗi khi phải tạo lại logic nhiều lần


