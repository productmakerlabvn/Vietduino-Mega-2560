# Mạch Vietduino Mega 2560 (Arduino Mega2560 Compatible)

![](/image/vmega_01.jpg)

## Giới thiệu

Mạch Vietduino Mega 2560 (Arduino Mega 2560 Compatible) được nghiên cứu và và sản xuất bởi MakerLab.vn dựa trên nguyên mẫu là mạch Arduino Mega 2560 với các ưu điểm vượt trội:

1. Thiết kế tương thích hoàn toàn về hình dạng, chuẩn chân tín hiệu và cách sử dụng với Arduino Mega 2560.
1. Sử dụng mạch nguồn xung giảm áp với ưu điểm là hiệu suất chuyển đổi cao, toả nhiệt thấp, tiết kiệm năng lượng, dải điện áp đầu vào cấp cho mạch rộng từ 6~24VDC với dòng đầu ra lớn: 5VDC/Max 1500mA, 3.3VDC / Max 700mA.
1. Bổ sung thêm các chân cấp nguồn POWER+ 5VDC giúp dễ dàng cấp nguồn cho nhiều thiết bị khác nhau.
1. Sử dụng IC chuyển đổi USB-UART CH340 được nhập khẩu chính hãng cho độ ổn định và độ bền cao.
1. Chức năng cách ly nguồn cổng USB tự động khi cấp nguồn ngoài từ chân Vin hoặc giắc DC giúp bảo vệ cổng USB máy tính của bạn an toàn hơn.

## Thông số kỹ thuật

<table><thead>
  <tr>
    <th>Model</th>
    <th>Mạch Vietduino Mega 2560 (Arduino Mega 2560 Compatible)</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Vi điều khiển</td>
    <td>ATMEGA2560-16AU</td>
  </tr>
  <tr>
    <td>Điện áp hoạt động</td>
    <td>5VDC</td>
  </tr>
  <tr>
    <td>Điện áp đầu vào VIN</td>
    <td>6~24VDC</td>
  </tr>
  <tr>
    <td>Digital I/O</td>
    <td>54 chân (D0-D53)</td>
  </tr>
  <tr>
    <td>PWM Digital I/O</td>
    <td>15 chân (D2-D13, D44-D46)</td>
  </tr>
  <tr>
    <td>Analog Input</td>
    <td>16 chân (A0-A15)</td>
  </tr>
  <tr>
    <td>Dòng DC đầu ra các chân I/O</td>
    <td>20mA</td>
  </tr>
  <tr>
    <td>Dòng DC đầu ra chân 3V3</td>
    <td>Max 700mA</td>
  </tr>
  <tr>
    <td>Dòng DC đầu ra chân 5V</td>
    <td>Max 1500mA</td>
  </tr>
  <tr>
    <td>Flash Memory</td>
    <td>256KB of which 8 KB used by bootloader</td>
  </tr>
  <tr>
    <td>SRAM</td>
    <td>8KB</td>
  </tr>
  <tr>
    <td>EEPROM</td>
    <td>4KB</td>
  </tr>
  <tr>
    <td>Clock Speed</td>
    <td>16MHz</td>
  </tr>
  <tr>
    <td>LED_BUILTIN</td>
    <td>D13</td>
  </tr>
  <tr>
    <td>BUTTON_BUILTIN</td>
    <td>S8 (D8)</td>
  </tr>
  <tr>
    <td>IC nạp chương trình và giao tiếp UART</td>
    <td>CP2102</td>
  </tr>
  <tr>
    <td>Cổng giao tiếp máy tính</td>
    <td>USB-B</td>
  </tr>
  <tr>
    <td>Kích thước</td>
    <td>101.6 x 53.35mm</td>
  </tr>
</tbody></table>

## Kích thước

![](/image/vmega_02.jpg)

## Hình ảnh sản phẩm

![](/image/vmega_03.jpg)
![](/image/vmega_04.jpg)

## Hướng dẫn sử dụng với phần mềm Arduino

### Hướng dẫn sử dụng phần mềm Arduino cơ bản

1) Giới thiệu về Arduino

2) Ngôn ngữ lập trình Arduino

3) Cách cài đặt phần mềm Arduino IDE

4) Cách cài đặt Driver và nạp chương trình cho mạch Arduino / Arduino Compatible

5) Cách cài đặt các thư viện phần cứng Arduino Library

6) Cách sử dụng Serial Monitor & Serial Plotter trên phần mềm Arduino

### Hướng dẫn kết nối và nạp chương trình cho Mạch Vietduino Mega 2560 trên phần mềm Arduino

1) Kết nối máy tính: Kết nối Mạch Vietduino Mega 2560 với máy tính bằng cáp USB sẽ thấy Led nguồn PWR trên mạch phát sáng.

2) Cài đặt Driver: Mạch Vietduino Mega 2560 mà một mạch Arduino Mega 2560 Compatible (tương thích Arduino Mega 2560) sử dụng IC nạp chương trình và giao tiếp máy tính CP2102, các bạn có thể tham khảo Hướng dẫn cài đặt Driver cho các mạch sử dụng IC giao tiếp USB-UART CP210x - MakerLab Wiki.

3) Cấu hình mạch trên phần mềm Arduino: Để cấu hình mạch trên phần mềm Arduino chúng ta cần làm các bước sau:

- Thiết lập Board tại Tools > Board > Arduino AVR Boards > Arduino Mega or Mega 2560 và Port (cổng kết nối) cho mạch, nếu không xác định được cổng kết nối có thể ngắt kết nối mạch và kết nối lại đồng thời kiểm tra phần Port để thấy cổng kết nối mới của mạch xuất hiện:
![](/image/vmega_05.jpg)
- Sau khi đã hoàn thành các thiết lập cơ bản bạn có thể nạp chương trình Blink sau vào mạch để test bằng cách nhấn vào nút Upload hoặc chọn Sketch > Upload sẽ thấy Led được kết nối với chân D13 trên mạch chớp tắt 1 giây 1 lần:

```ino
/*
  Blink
  Turns an LED_BUILTIN on D13 of Vietduino Mega 2560 for one second, then off for one second, repeatedly.
*/
// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN on D13 as an output.
  pinMode(13, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(13, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(13, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
```

![](/image/vmega_06.jpg)

## Nhà phân phối

Có thể mua Mạch Vietduino Mega 2560 tại các nhà phân phối sau:

- [Hshop.vn - Điện tử & Robot.](https://hshop.vn)
