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

# 2. Viết app sử dụng Android Studio
## Android Cơ Bản - Ghi Chú Tổng Hợp
## 1. AndroidManifest.xml là gì?

`AndroidManifest.xml` là file cấu hình quan trọng nhất của ứng dụng Android.

File này dùng để mô tả thông tin cơ bản của ứng dụng như:

* Tên package
* Activity của ứng dụng
* Quyền (Permission)
* Theme
* Icon
* Version ứng dụng

Ví dụ cấu trúc Manifest:

```xml
<manifest xmlns:android="http://schemas.android.com/apk/res/android">

    <application
        android:allowBackup="true"
        android:theme="@style/Theme.MyApp">

        <activity android:name=".MainActivity"/>

    </application>

</manifest>
```

### Mục đích

Giúp Android hiểu ứng dụng gồm những thành phần nào và ứng dụng cần quyền gì để hoạt động.

---

## 2. App cần quyền để thực hiện chức năng

Một số chức năng trong Android yêu cầu cấp quyền trước khi sử dụng.

Ví dụ:

* Internet
* Camera
* Vị trí GPS
* Bộ nhớ
* Micro

### Khai báo quyền trong Manifest

Ví dụ cấp quyền Internet:

```xml
<uses-permission android:name="android.permission.INTERNET"/>
```

Ví dụ cấp quyền Camera:

```xml
<uses-permission android:name="android.permission.CAMERA"/>
```

### Mục đích của Permission

* Đảm bảo bảo mật cho người dùng
* Tránh ứng dụng truy cập trái phép dữ liệu cá nhân
* Android yêu cầu người dùng đồng ý trước khi cấp quyền

---

## 3. Vòng đời của ứng dụng Android

Một ứng dụng Android hoạt động theo vòng đời (Lifecycle).

Các hàm quan trọng gồm:

* `onCreate()`
* `onStart()`
* `onResume()`
* `onPause()`
* `onStop()`
* `onDestroy()`

### Ý nghĩa từng hàm

#### onCreate()

Được gọi khi Activity vừa được tạo.

Thường dùng để:

* Khởi tạo giao diện
* Ánh xạ View
* Khởi tạo dữ liệu

Ví dụ:

```java
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
}
```

---

#### onStart()

Được gọi khi Activity bắt đầu hiển thị.

---

#### onResume()

Được gọi khi người dùng bắt đầu tương tác với ứng dụng.

---

#### onPause()

Được gọi khi ứng dụng bị tạm dừng.

Ví dụ:
Người dùng chuyển sang ứng dụng khác.

---

#### onStop()

Được gọi khi ứng dụng không còn hiển thị.

---

#### onDestroy()

Được gọi khi Activity bị đóng hoàn toàn.

---

## 4. Tại sao project mới có sẵn hàm onCreate()?

Sau khi tạo project mới, Android Studio tự sinh sẵn:

```java
protected void onCreate(Bundle savedInstanceState)
```

Lý do:

Android sẽ tự động gọi hàm này khi Activity được khởi tạo.

Do đó lập trình viên thường đặt code khởi tạo trong `onCreate()`.

Ví dụ:

```java
setContentView(R.layout.activity_main);
```

Dùng để gắn giao diện XML vào Activity.

---

## 5. Kiểm tra quyền bằng Java

Ngoài khai báo trong Manifest, Android còn yêu cầu kiểm tra quyền bằng code.

Ví dụ kiểm tra quyền Camera:

```java
if(ContextCompat.checkSelfPermission(
        this,
        Manifest.permission.CAMERA)
        != PackageManager.PERMISSION_GRANTED){

    ActivityCompat.requestPermissions(
            this,
            new String[]{
                    Manifest.permission.CAMERA
            },1);
}
```

### Ý nghĩa

* Kiểm tra xem ứng dụng đã có quyền chưa
* Nếu chưa sẽ yêu cầu người dùng cấp quyền

---

## 6. Giao diện Android bằng XML

Giao diện Android được thiết kế trong thư mục:

```text
res/layout
```

Ví dụ:

```text
activity_main.xml
activity_second.xml
```

Android hỗ trợ hai cách xây dựng giao diện:

* **XML Code**
* **Design View**

### XML

Viết giao diện bằng code XML.

Ví dụ:

```xml
<Button
    android:id="@+id/btnTinh"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Tính"/>
```

### Design View

Thiết kế giao diện bằng kéo thả trực tiếp.

---

## 7. Hardcode và Resource

Không nên hardcode text trực tiếp trong XML.

Ví dụ không nên:

```xml
android:text="Xin chào"
```

Nên lưu trong:

```text
res/values/strings.xml
```

Ví dụ:

```xml
<string name="hello">Xin chào</string>
```

Sau đó tham chiếu:

```xml
android:text="@string/hello"
```

### Cú pháp tham chiếu

```text
@string/tên_biến
```

Ví dụ:

```text
@string/hello
```

---

## 8. Ưu điểm của việc tham chiếu Resource

* Dễ thay đổi nội dung
* Không phải sửa nhiều nơi
* Dễ quản lý text
* Hỗ trợ đa ngôn ngữ

Ví dụ:

```text
values-vi
values-en
```

Android sẽ tự động đổi ngôn ngữ.

---

## 9. LOCATION, LANGUAGE, THEME

Android hỗ trợ tự động lấy giá trị phù hợp với:

* **Location**
* **Language**
* **Theme**

Ví dụ:

Người dùng chọn English:

Ứng dụng tự lấy:

```text
values-en
```

Người dùng chọn tiếng Việt:

Ứng dụng tự lấy:

```text
values-vi
```

### Ý nghĩa

Giúp ứng dụng hiển thị phù hợp với:

* Quốc gia
* Ngôn ngữ
* Giao diện người dùng

---

## 10. Đối tượng chứa (Layout Container)

Container là đối tượng dùng để chứa các component con.

Ví dụ:

* `LinearLayout`
* `ConstraintLayout`
* `RelativeLayout`

### LinearLayout

Dùng để sắp xếp component theo:

#### Chiều dọc

```xml
android:orientation="vertical"
```

#### Chiều ngang

```xml
android:orientation="horizontal"
```

---

### Gravity

Dùng để căn chỉnh vị trí component.

Ví dụ:

```xml
android:gravity="center"
```

Ý nghĩa:
Canh giữa nội dung.

---

## 11. Code tương tác với Layout

Ví dụ hiển thị text:

```java
TextView tv;

tv = findViewById(R.id.txtHello);

tv.setText(getString(R.string.hello));
```

### Ý nghĩa

Sử dụng:

```java
getString()
```

để tránh hardcode và hỗ trợ đa ngôn ngữ.

---

## 12. Hiển thị text phù hợp Language, Theme, Location

Để text phù hợp với thiết lập của người dùng cần:

### Không hardcode text

Ví dụ không nên:

```java
tv.setText("Xin chào");
```

Nên dùng:

```java
tv.setText(getString(R.string.hello));
```

### Mục đích

* Hỗ trợ nhiều ngôn ngữ
* Tự động đổi theo hệ điều hành
* Dễ quản lý nội dung

---

## 13. Event trong Android

Event là hành động của người dùng tác động vào ứng dụng.

Ví dụ:

* Click Button
* Click Text
* Click Image

---

## 14. Xử lý sự kiện bằng 2 cách

### Cách 1: Dùng XML

Trong Layout:

```xml
android:onClick="clickButton"
```

Trong Java:

```java
public void clickButton(View view){

}
```

### Ý nghĩa

Khi người dùng click button sẽ gọi hàm `clickButton()`.

---

### Cách 2: setOnClickListener

Trong Java:

```java
Button btn;

btn = findViewById(R.id.btnTinh);

btn.setOnClickListener(v -> {

});
```

### Ý nghĩa

Khi click button sẽ thực hiện đoạn code bên trong.

---

## 15. Thư mục Assets trong Android

Assets là thư mục đặc biệt dùng để chứa dữ liệu đi kèm ứng dụng.

Ví dụ:

* JSON
* TXT
* HTML
* Image
* Video

Khi build APK, toàn bộ file trong Assets sẽ đi theo ứng dụng.

### Lợi ích

* Hoạt động offline
* Không cần Internet
* Truy cập dữ liệu nhanh

---

## 16. Truy cập file trong Assets

Ví dụ đọc file:

```java
InputStream inputStream =
        getAssets().open("data.json");
```

### Ý nghĩa

Cho phép ứng dụng truy cập dữ liệu đã đóng gói sẵn trong app.

---

## 17. Ứng dụng của Assets

Ví dụ:

Ứng dụng hướng dẫn món ăn Việt Nam.

Dữ liệu:

```text
monan.json
```

chứa:

* tên món ăn
* mô tả
* hình ảnh

Ứng dụng có thể hoạt động kể cả khi không có Internet.

### Ưu điểm

* Offline hoàn toàn
* Không phụ thuộc server
* Dữ liệu luôn sẵn trong ứng dụng
# Tạo app 1
- Tạo Project mới trong Android Studio

- File → New → New Project → Empty Views Activity

<img width="1127" height="817" alt="image" src="https://github.com/user-attachments/assets/8cbfb6f0-8ca1-497e-beaa-2743c2cf8001" />

Tạo thư mục Assets

<img width="603" height="463" alt="image" src="https://github.com/user-attachments/assets/32696e29-a927-4452-badb-0735cedbb34d" />

- Tạo file foods.json: Click chuột phải vào thư mục assets vừa tạo → New → File → đặt tên foods.json image
  
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e2c773fb-f16b-4b2d-b29d-a738e2fc0993" />

- Thiết kế giao diện (activity_main.xml)
  
    + Mở res/layout/activity_main.xml

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/890d1b44-a71c-4907-a902-dfb0f33f3899" />

- Viết code Java (MainActivity.java)
    + Mở MainActivity.java

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1b4b374b-0858-44e5-a9fd-ea461d4488f3" />

mở file res/values/strings.xml

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/80e20e36-0d82-4c7a-bb8d-004fb2c91811" />

- Chạy Bài

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/955c3ea4-40b5-4304-ad07-eac782b94453" />

Test thử chức năng

- Ấn vào cao lấu sẽ ra như dưới
- 
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c08a6951-b8a0-48f5-b5ff-59e28707d0d8" />

- Gõ tên tỉnh TP.HCM thì nó sẽ ra món ăn ở tỉnh đó là bánh mì
  
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/230409f4-7552-4dba-9755-0316fccd4469" />

- Chọn Hà nội thì nó sẽ hiện thị các mon đặc trưng của Hà Nội

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0d09a4e6-c83c-42cc-bf94-b58432cdd98a" />

Tạo app 2(android studio): tạo app tương đương với Mit App inventor

- Tạo Project mới trong Android Studio

   + File → New → New Project → Empty Views Activity

<img width="1140" height="819" alt="image" src="https://github.com/user-attachments/assets/f65965ad-3c28-4d31-9540-08196e927c41" />

- Tạo thêm Activity 1 , Activity 2 và Activity 3
 + cột thư mục bên trái (tab Project), tìm đường dẫn: app -> java -> com.example.app2mitinventor
 + Chuột phải vào thư mục tên package đó -> Chọn New -> Activity-> Empty Views Activity.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/28bb23ae-dd9c-4977-9f0d-40e39791e441" />

- Tạo AboutActivity, MathActivity và WebActivity

<img width="594" height="484" alt="image" src="https://github.com/user-attachments/assets/f108fe29-4d1c-4bee-8f0f-97f3b4a95082" />

Cấu hình Quyền Internet trong Manifest
Mở file app -> manifests -> AndroidManifest.xml.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dc051786-5e07-4cd5-a406-de3433d6f031" />

Viết code cho Màn hình 1 (About + Điều hướng)

Giao diện: Mở file res -> layout -> activity_about.xml

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9cf27502-1d83-4b9d-8808-aa48f981d331" />

Logic: Mở file MainActivity.java.

Viết code ánh xạ nút bấm và dùng lệnh Intent để khi click nút 1 sẽ mở Activity2, click nút 2 sẽ mở Activity3

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4888e68c-56bc-4d99-99d4-cc7d2e229bb6" />

Viết code cho Màn hình 2 (Giải toán + Gọi API) + Giao diện: Mở file res -> layout -> activity_math.xml. Viết code thiết kế gồm 3 ô nhập dữ liệu (EditText cho a, b, c), 1 nút bấm "GIẢI TOÁN" và 1 TextView hiện kết quả.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b67a4ded-ae7c-4f58-932f-b0cfcc2d7563" />

Logic Xử lý mạng & Toán học: MathActivity.java

Mở file MathActivity.java.

Viết hàm giải phương trình khi ấn nút.

Tạo một luồng chạy nền bằng ExecutorService để đóng gói dữ liệu thành chuỗi JSON lồng nhau (Nested JSON) theo đúng cấu trúc: {app_by, input: {...}, output: {...}}.

Thực hiện kết nối HttpURLConnection, đẩy dữ liệu theo phương thức POST lên địa chỉ https://k58kmt.tdh.io.vn/api.

Nhận kết quả phản hồi {ok:1, stt:1234} từ Server và hiển thị lên màn hình.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/88e1417f-d519-4863-9042-9d4bcb3e97b6" />

Viết code cho Màn hình 3 (WebView Định danh)

Giao diện: Mở file res -> layout -> WebActivity.xml. Thêm duy nhất một linh kiện chiếm toàn màn hình (match_parent).

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/05564346-c545-4a5a-9ed0-2ad7a776628a" />

Logic: Mở file  WebActivity.java.

Kích hoạt JavaScript (setJavaScriptEnabled(true)).

Tạo chuỗi URL động bằng cách nối mã sinh viên vào đuôi: "https://k58kmt.tdh.io.vn?masv=" + MA_SINH_VIEN.

Gọi lệnh loadUrl() để tải trang web ngay trong ứng dụng.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/67fe9a4c-7b14-4bef-ae13-37caf4ea94aa" />

## Chạy thử và kiểm tra 

- Test màn 1: Kiểm tra xem thông tin cá nhân đã chuẩn chưa. Ấn nút 1 xem có nhảy sang màn 2 không.
  
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0891b706-24a2-48fd-b4f9-d4c1d3c9b48a" />

- ấn nút giải phương trình thì nhảy sang màn hình 2

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f1e6cede-38f1-4166-bd99-2daae2b93671" />

**Em thừa thầy, phần code gọi API POST dữ liệu và WebView của em đã viết chuẩn cấu trúc, nhưng do server k58kmt.tdh.io.vn hiện đang sập (hoặc không truy cập được từ mạng ngoài) nên app nhảy vào nhánh báo lỗi kết nối ạ.**

<img width="960" height="1018" alt="image" src="https://github.com/user-attachments/assets/3786a4e6-b7e5-4d6c-beee-8d4e73782a3a" />

Test màn 3: Ấn nút mở WebView xem trang web có tải mượt mà và nhận đúng mã sinh viên ở thanh địa chỉ không.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4408fd06-904a-4c29-b539-f975b8b01377" />

-  Do tên miền k58kmt.tdh.io.vn thực sự đang sập hoặc không tồn tại. Tuy nhiên dòng chữ nhỏ trên màn hình máy ảo, nó ghi là: The webpage at https://k58kmt.tdh.io.vn/?masv=K225480106040 could not be loaded... Điều này chứng tỏ code WebView định danh đã chạy đúng 100%!.Ứng dụng đã gọi đúng linh kiện trình duyệt. Ứng dụng đã tự động tạo chuỗi, ghép thành công mã số sinh viên K225480106040 vào đuôi URL một cách chuẩn xác đúng như yêu cầu của đề bài. Việc web không hiện ra chỉ đơn thuần là do máy chủ đang đóng cửa server. **
