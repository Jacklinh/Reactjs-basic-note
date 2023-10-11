# Session 01: JavaScript

Chúng ta ôn lại các kiến thức sau:

> 🔸 Variables- biến(let, const, var)

> 🔸 Arrow Function

> 🔸 Javascript Classes

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



