# Session 01: JavaScript

Chúng ta ôn lại các kiến thức sau:

> 🔸 Variables- biến(let, const, var)

> 🔸 Arrow Function

> 🔸 The for/of loop- vòng lặp

> 🔸 Array map

***

## 🔶  Variables- biến

> 🔸 Quy tắc đặt tên biến

- các keywords trong javascript: <https://www.w3schools.com/js/js_reserved.asp>
- đặt tên theo kiểu camleCase(lạc đà): như tên cách viết của nó, từ đầu tiên viết thường, các từ tiếp theo viết HOA  chữ cái đầu tiên. EX: myName...
- Đặt tên theo underscore: sử dụng dấu gạch chân dưới (_) giữa các từ, tất cả đều viết thường. EX: my_name...
- Đặt tên theo PascalCase: Viết hoa tất cả các chữ cái đầu. EX: MyName...

> 🔸 let

- Tạo ra 1 biến chỉ có thể truy cập được trong block bao quanh nó (block scope). 
- khác với var nó phạm vi truy cập xuyên suốt function chứa nó(global scope)

```js
var x = 100;
//here x is 100
{
    let x = 8;
    // here x is 8
}
// here x is 100
```
> 🔸 const
- dùng để khai báo 1 hằng số - là 1 giá trị không thay đổi được trong quá trình chạy
- như let thì const cũng là 1 block scope

***

## 🔶  Arrow function

- cú pháp truyền thống

```js
function sum(a, b) { // hàm trả về giá trị với câu lệnh return
    return a + b;
}
let result = sum(5,8);
console.log('result sum', result);
```

- ES5 , function không tên

```js
let result = function (a, b) { // hàm trả về giá trị với câu lệnh return
    return a + b;
}
```
- ES6: arrow function short hand

```js
let result = (a, b) => { // bỏ function thay =>
    return a + b;
}
// với trả về 1 giá trị thì ta có thể viết rút gọn hơn như sau
let result = (a, b) => a + b; // bỏ dấu {} và return đi
```

***

## 🔶  The for/of loop- vòng lặp

** for **

Khái niệm 

- vòng lặp `for` là 1 cấu trúc điều kiện, nó cho phép thực hiện 1 tập hợp các câu lệnh lặp lại 1 số lần xác định hoặc lặp qua các phần tử trong 1 cấu trúc dữ liệu như array... ==> với `for`bạn có thể kiểm soát rõ ràng số lần lặp và có thể truy cập vào các chỉ số(index) hoặc giá trị(value) của 1 phần tử 1 cách dễ dàng
```js
    for(innitialization; condition; iteration){
        // các câu lệnh được lặp lại
    }
```
Giải thích cú pháp

-`initialization`: khởi tạo giá trị ban đầu cho biến đếm, dùng let or var

- `condition`: điều kiện kiểm tra TRƯỚC mỗi lần lặp, nếu điều kiện này đúng thì khối mã bên trong vòng lặp sẽ thực thi. còn sai thì vòng lặp kết thúc.

- `iteration`: câu lệnh được thực hiện sau mỗi vòng lặp. thường là 1 câu lệnh để tăng hoặc giảm giá trị biến đếm

Quá trình hoạt động

1. bước khởi tạo: Phần `initialization` khởi tạo được thực hiện 1 lần duy nhất khi vòng lặp bắt đầu. Nó được sử dụng để khởi tạo biến đếm và thiết lập giá trị ban đầu.

2. Kiểm tra điều kiện sau: sau mỗi lần lặp, điều kiện kiểm tra luôn được kiểm tra. Nếu đúng thì khối mã bên trong vòng lặp được thực thì, còn sai thù vòng lặp kết thúc và quá trình tiếp tục với các câu lệnh sau vòng lặp

3. thực thi khối mã: trong mỗi lần lặp, khối mã bên trong vòng lặp sẽ được thực thi.

4. Bước lặp: sau khi thực thi khối mã, bước lặp được thực hiện.Thông thường nó là 1 câu lệnh để tăng hoặc giảm giá trị của biến đêm. sau đó quá trình quay lại bước kiểm tra điều kiện

** for...in **

Khái niệm 

- vòng lặp `for...in` là 1 cấu trúc điều kiện dùng để lặp qua các thuộc tính của đối tượng và thực thi 1 khối mã tương ứng, thường dùng lặp qua 1 Object

```js
for(variable in object) {
    // các câu lệnh được lặp lại
}
```

Giải thích cú pháp

- `variable`: biến mà bạn sẽ sử dụng để lưu trữ tên của từng thuôc tính trong đối tượng. trong mỗi lần lặp, giá trị của biến này sẽ thay đổi thành tên thuộc tính hiện tại
` object`: là đối tượng mà bạn muốn lặp qua các thuộc tính của nó

Quá trình hoạt động

1. mỗi lần thuộc tính của đối tượng được lặp qua 1 cách tuần tự

2. trong mỗi lần lặp, tên thuộc tính được gán cho biến `variable`

3. khối mã bên trong vòng lặp được thực thi

4. Quá trình lặp tiếp tục cho đến khi tất cả các thuộc tính của đối tượng ddaxx được lặp qua.


** for...of **

Khái niệm 

- vòng lặp `for...of` là 1 cấu trúc điều kiện dùng để lặp qua các phần tử của 1 đối tượng CÓ KHẢ NĂNG LẶP LẠI(iterable), chẳng hạn như array, object, hoặc 1 Dom( 1 đối tượng Giao diện người dùng)

```js
for(variable of iterable) {
    // các câu lệnh được lặp lại
}
```

Giải thích cú pháp

- `variable`: là biến mà bạn sẽ sử dụng để lưu trữ giá trị của từng phần tử của đổi tượng có khả năng lặp lại
- `iterable`: là đối tượng có khả năng lặp lại mà bạn muốn lặp qua các phần tử của nó.

Quá trình hoạt động

1. vòng lặp sẽ lặp qua từng phần tử của đối tượng có khả năng lặp lại

2. trong mỗi lần lặp, giá trị của phần tử được gán cho biến `variable`

3.  khối mã bên trong vòng lặp được thực thi

4. quá trình lặp tiếp tục cho đến khi tất cả các phần tử của đối tượng đã được lặp qua.

> 🔸 Array 

- array for, for/in, for/of

```js
const colorsArr = ['black','white','blue','yellow'];
const lengthColor = colorsArr.length; // 4 - đếm mảng có bao nhiêu phần tử
// dùng for với điều kiện đúng : mỗi lần lặp qua, tăng index lên 1
for(let index = 0; index < lengthColor; index++) {
    console.log('index: ',index); // vị trí của phần tử băt đầu từ 0
    console.log('value: ',colorsArr[index]); //truy cập giá trị của phần tử dựa vào index
}

// dùng for/in lặp qua key của đối tượng để lấy giá trị
for(let index in colorsArr) {
    console.log(`value index ${index} - ${colorsArr[index]}`)
}
// dùng for/of lặp qua value của đối tượng => return value 
for(let value of colorsArr) {
    console.log(`value  ${value} `)
}
```
- Array.forEach()

> 🔸 String

```js
let language = 'javascript';
let text = '';
for(let x of language) {
    text += x + '';
    console.log('text',text)
}
```
> 🔸 Object

```js
    const person = {
        fname: 'Anh',
        lname: 'van',
        age: '20'
    };
    for(let key in person){
        console.log(key + ": " + person[key]);
        // output here:
        // fname: Anh
        // lname: van
        // age 20
    }
```
> 🔸 Array.forEach() 

- `forEach` là phương thức lặp qua từng phần tử của ARRAY theo thứ tự tăng dần mà không làm thay đổi kết cấu của mảng.

```js
forEach(callbackFn, [thisArg]){
    // các câu lệnh 
}
```

Giải thích cú pháp
nhận vào 1 `callbackFn` làm nhiệm vụ lặp qua từng phần tử của mảng được cung cấp, có 3 tham số chính được cung cấp là : 
- `item`: Giá trị của các phần tử trong mảng

- `index`: vị trí của phần tử trong mảnh

`array`: mảng gốc đang được lặp từ forEach

còn `thisArg` là biến có thể có hoặc không và lấy giá trị của dối tượng ra ngoài forEach
