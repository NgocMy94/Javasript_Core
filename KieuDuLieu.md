Các kiểu dữ liệu trong JavaScript
1. Kiểu dữ liệu là gì?

Kiểu dữ liệu (data type hoặc chúng ta có thể gọi đơn giản là type) là một cách để phân loại dữ liệu cho trình biên dịch hiểu các lập trình viên muốn sử dụng loại dữ liệu nào.

JavaScript cho phép chúng ta làm việc với các kiểu dữ liệu nguyên thủy (string, number,…) và kiểu dữ liệu không nguyên thủy.

Kiểu dữ liệu nguyên thủy:

Number: Các số nguyên hoặc số thực. Ví dụ: 5 hoặc 5.05
String: là các text như “Các kiểu dữ liệu trong JavaScript”, text có thể có một hoặc nhiều ký tự.
Boolean: chỉ có 2 giá trị là true hoặc false.
Undefine:  là các giá trị không xác định.
Null: đơn giản là không có giá trị nào cả.

Kiểu dữ liệu không nguyên thủy (tham chiếu):

Object: Thể hiện một đối tượng và các thuộc tính có thể truy cập đến.
Array: Nhóm các giá trị giống nhau.
RegExp: Biểu thức chính quy.

Bởi vì các kiểu dữ liệu không nguyên thủy phức tạp hơn nên sẽ được hướng dẫn cụ thể hơn trong các bài học sau.

Bài viết này chúng ta sẽ tập trung vào các kiểu dữ liệu nguyên thủy trước.

2. Các kiểu dữ liệu nguyên thủy trong JavaScript
2.1. Kiểu dữ liệu String
String là kiểu dữ liệu chứa dữ liệu dưới dạng text. Kiểu string trong JavaScript cho phép bạn sử dụng cả ngoặc đơn và ngoặc kép để biểu diễn nó.

Ví dụ, chúng ta tạo một file .js và có đoạn code sau:

let name = 'NIIT - ICT Hà Nội'; // Chuỗi trong dấu ngoặc đơn.
let action = ' hướng dẫn học ';
let JS = "JavaScript"; //Chuỗi trong dấu nháy kép.

2.2. Kiểu dữ liệu Number

Kiểu dữ liệu number trong JavaScript có thể xem là kiểu tổng hợp của int, float, double, … trong các ngôn ngữ lập trình khác.

Hiểu đơn giản number là kiểu dữ liệu số, số nguyên, số thực,… đều là kiểu số cả.

let number1 = 10;
// Gán giá trị number1 = 10, number1 là kiểu number.
let number2 = 10.05;
document.writeln(number1);
// Hiển thị number1 ra trình duyệt.
document.writeln(number2);
// Hiển thị numbwer2 ra trình duyệt.
document.writeln(number1 + number2);
//Hiển thị tổng của hai số ra trình duyệt.

Ở trên là các biến number1 là số nguyên, number2 là số thực.

Ta có thể thực hiện number1 + number2 bởi vì nó đều là kiểu number, không phân biệt là số, số thực, số nguyên gì cả, có thể thực hiện tất cả các phép toán.

> Lưu ý #3: Trong kiểu Number này bạn cần lưu ý hai giá trị đặc biệt:

Infinity: Là số “vô cực” trong toán học.
NaN: Là Not a Number, tức là giá trị này không phải là số

2.3. Kiểu dữ liệu Boolean

Trong JavaScript, các kiểu dữ liệu thuộc kiểu dữ liệu boolean chỉ có thể nhận một trong hai giá trị, đó là:

true: Đúng
false: Sai

Có hai cách để nhận giá trị kiểu boolean:

Gán giá trị trực tiếp

let a = true;
let b = false;
 
Nhận kết quả từ một biểu thức

let c = 10 > 11;
let d = 10 < 15;
 
Để kiểm chứng, chúng ta hiển thị giá trị của các biến này ra xem sao nhé:

document.writeln(a);
document.writeln(b);
document.writeln(c);
document.writeln(d);
// Kết quả: true false false true
 
Kiểu dữ liệu boolean thường được sử dụng trong các câu lệnh rẽ nhánh.

2.4. Kiểu dữ liệu undefined

Trong JavaScript, khi một biến được khai báo mà không gắn với bất kỳ giá trị nào thì biến đó gọi là kiểu dữ liệu undefined, giá trị cũng là undefined luôn. (Như bạn đã thấy ở bài Biến trong JavaScript)


// Biến này chưa đượcgán giá trị
// Do đó nó chứa giá trị mặc định là undefined
let undef; 
// Kiểu dữ liệu của nó lúc này là undefined
document.write(typeof undef);
// Kết quả: undefined
 

2.5. Kiểu dữ liệu Null

Trong JavaScript hỗ trợ kiểu dữ liệu null, có nghĩa là không có gì, bạn chỉ cần khai báo biến bằng null là có thể sử dụng kiểu này.


let bienNull = null;
 

Đơn giản phải không? :D

Nhưng vấn đề này mới làm đau đầu bao nhiêu chuyên gia lập trình đây này.


document.write(bienNull);   
// Kết quả: null
 

Và...


document.write(typeof bienNull);
// Kết quả: Object
 

Phân biệt kiểu undefined và kiểu null như thế nào?

Nhiều bạn sẽ nhầm lẫn giữa hai kiểu dữ liệu này. Các bạn nghĩ hai kiểu này đều nói về một biến không xác định đúng không nào?


Nó không hẳn là vậy.

Một biến được khai báo mà không gán giá trị khởi tạo thì JavaScript sẽ đặt cho nó giá trị mặc định là undefined, kiểu dữ liệu cũng là undefined.
Khi bạn kiểm tra kiểu dữ liệu bằng từ khóa typeof thì sẽ ra kiểu dữ liệu và undefined. Còn với null, nó có nghĩa là không có gì. Nhưng sự khác biệt là mặc dù biến đó không có giá trị nhưng kiểu dữ liệu của nó là object.
