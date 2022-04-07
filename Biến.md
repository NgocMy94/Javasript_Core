1 Biến trong JavaScript

* Biến dùng để lưu trữ giá trị các dữ liệu, hay các đối tượng. Giá trị của biến tùy bạn thay đổi trong quá trình chương trình làm việc để đáp ứng yêu cầu riêng của bạn.

Trong JavaScript có hai kiểu khai báo biến là let và var.

1.1. Khai báo biến với từ khóa var

Cú pháp khai báo biến trong JavaScript bằng từ khóa var:

var ten_Bien_A, ten_Bien_B, ...;

Trong đó:
var: từ khóa khai báo biến.
ten_Bien_A, ten_Bien_B, … là danh sách tên biến. Bạn cũng có thể chỉ khai báo 1 biến.

1.2. Khai báo biến với từ khóa let

Cú pháp khai báo biến trong JavaScript bằng từ khóa let:


let ten_Bien_A, ten_Bien_B, ...;
 


Trong đó:

let: từ khóa khai báo biến.
ten_Bien_A, ten_Bien_B, … là danh sách tên biến. Bạn cũng có thể chỉ khai báo 1 biến.

1.3. Sự khác nhau của từ khóa let và var

Đối với biến khai báo bằng từ khóa var:



// Khi khai báo bằng var thì biến đó có thể được
// khai báo lại sau khi đã được khai báo trước đó.
var x = 5;
// ...
var x = 10; // Khai báo lại sẽ không có vấn đề gì
 

Đối với biến khai báo bằng từ khóa let:


// Khi khai báo bằng let thì biến đó không được khai báo nữa.
let x = 5;
//….
let x = 10; // Khai báo lại sẽ báo lỗi
 

Tóm lại , khai báo bằng let và var khác nhau:

var cho phép khai báo lại một biến, let thì biến chỉ được khai báo 1 lần, nếu khai báo lại sẽ bị lỗi.
Biến được khai báo bằng let thì phạm vi hiệu lực trong khối lệnh { } mà nó khai báo, var thì hiệu lực toàn cục.

> Lưu ý: JavaScript hỗ trợ cả gán giá trị cho biến khi khai báo và gán giá trị sau khi khai báo.

// Vừa khai báo vừa gán giá trị
let x = 10;

// Khai báo biến
let y;
// Gán giá trị cho biến
y = 10;

4. Cách đặt tên biến trong JavaScript

Đặt tên biến là một việc cực kỳ quan trọng trong lập trình, đặt tên biến tốt sẽ giúp chương trình của bạn không bị lỗi, khả năng đọc tốt, dễ dàng duy trì và phát triển sau này.

Quy tắc, cách đặt tên biến trong JS:

Trong JavaScript phân biệt chữ thường và chữ hoa. Nên biến x sẽ khác biến X.
Bắt đầu bằng một chữ cái hoặc _ hoặc $. Tiếp theo là chuỗi các ký tự chữ, số, gạch dưới, dollar
Không được bắt đầu bằng số
Không được chứa các ký hiệu toán học, logic ví dụ *, +,…
Không được chứa khoảng trắng

5. Hằng số trong JavaScript

Hằng số được khai báo phải khởi tạo ngay với từ khóa const, sau khi khai báo và gán thì giá trị sẽ không được thay đổi nữa.

Từ khóa const là trường hợp đặc biệt của biến.

Cú pháp:

const tenHangSo = giaTriHangSo;
 
Trong đó:

const: là từ khóa khai báo hằng số
tenHangSo: là tên của hằng số
giaTriHangSo: là giá trị của hằng số

Ví dụ:
const PI = 3.1415;
const BRAND = "NIIT - ICT HÀ NỘI";
 

