# Section 1 giới thiệu React

Trong section này chúng ta sẽ lần lượt tìm hiểu các vấn đề sau:
> 🔸 Reactjs là gì ?

> 🔸 Reactjs có phổ biến không?

> 🔸 Reactjs có thể làm gì?

> 🔸 Tại sao nên học Reactjs

> 🔸 Ôn lại Flexbox

> 🔸 Ôn lại Javascript Es6

> 🔸 Môi trường phát triển Reactjs (node js, npm/yarn)

> 🔸 Cài đặt Reactjs - hello reactjs

***

## 🔶  React là gì ?

- Reactjs là 1 thư viện Javascript, được sử dụng trong lập trình web tạo ra từ 1 kỹ sư Facebook - Jordan Walke vào năm 2011 nhằm tập trung vào mảng develop UI.
- Reactjs là 1 thư viện giao diện người dùng (UI)
- Reactjs là 1 công cụ xây dựng các UI component

Tuy nhiên, chúng ta ôn lại 1 chút về Javascript là gì? Thư viện Javascript là gì?

> 🔸 Javascript là gì?

- Javascript(JS) là 1 ngôn ngữ script, dùng để tạo và kiểm soát nội dung web động vd như đồ họa động, slideshow ảnh, show hide content...

> 🔸 Thư viện Javascript là gì? 

- là bộ sưu tập code Javascript, các code này có thể được sử dụng cho những tác vụ JS cơ bản. Cho phép bỏ qua quá trình thủ công viết code tốn thời gian, không cần thiết.
- Hiện nay có rất nhiều loại thư viện Javascript khác nhau và Reactjs chính là 1 trong số đó.

***

## 🔶  React có phổ biến không?

- Github Star(lượt tương tác rất cao): <https://github.com/facebook/react/>
- Google trend: <https://trends.google.com/trends/explore?q=%2Fm%2F012l1vxv,%2Fg%2F11c0vmgx5d,%2Fg%2F11c6w0ddw9>
- Các trang web sử dụng Reactjs: Facebook, Instagram, Netflix, Reddit, Uber, Airbnb, The New York Times, Khan, Academy, Codecademy, SoundCloud, Discord, WhatsApp Web...

***

## 🔶  Reactjs có thể làm gì?

- làm WEB app
- làm Mobile app
- Làm Destop app

***

## 🔶  Tại sao nên học Reactjs?

- Khả năng mở rộng và tái sử dụng cao
- Hiệu suất ứng dụng cao
- Phát triển nhanh( có thư viện hỗ trợ khổng lồ)
- Cơ hội việc làm cao và thu nhập cao
- Cộng đồng lớn
- Trend phát triển <https://trends.google.com/trends/explore?cat=31&date=2021-01-01%202023-07-17&q=Vue,React,Angular>

> 🔸 Xem Biểu đồ Trend tech: 
- <https://survey.stackoverflow.co/2023/#section-most-popular-technologies-web-frameworks-and-technologies>
- <https://npmtrends.com/@angular/core-vs-angular-vs-react-vs-vue>

> 🔸 Các điểm nổi bật trong Reactjs

- Phù hợp với đa dạng thể loại website: Reactjs khiến cho việc khởi tạo website dễ dàng hơn bởi vì bạn không cần phải code nhiều như khi tạo trang web thuần chỉ dùng javascript, html và nó đã cung cấp cho bạn đủ loại "đồ chơi" để bạn có thể dùng với nhiều trường hợp.
- Tái sử dụng các Component: Nếu bạn xấy dựng các component đủ tốt để có thể thỏa các "yêu vaaif" của nhiều dự án khác nhau, bạn chỉ tốn thời gian xây dựng ban đầu và sử dụng lại hầu như toàn bộ ở các dự án sau.
- Có thể sử dụng cho cả Mobile app: Ngoài sử dụng cho việc lập trình website, nó còn được sinh ra phát triển thêm ứng dụng MObile-kết hợp React Native
- Thân thiện với SEO: Bản chất Reactjs là 1 thư viện Javascript. Google search Engine hiện đã crawl(thu thsspj thông tin) và index được code javascript , tuy nhiên bạn cũng cần thêm 1 vào thư viện khác để hỗ trợ điều này!
- Debug dễ dàng. Facebook đã phát hành 1 chrome extension dùng cho việc debug trong quá trình phát triển ứng dụng ( React Developer Tools
)

***

## 🔶  Ôn lại Flexbox

xem các trang nguồn và ví dụ 

Cheat: -- <https://flex.eszter.space/>

Demo: <https://codepen.io/enxaneta/full/adLPwv/>

Flexbox Model (xem hình minh họa) -- <https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox#the_flex_model>

***

## 🔶  Ôn lại Javascript Es6

- Nắm thật chắc cú pháp ES6 : -- <https://www.w3schools.com/REACT/react_es6.asp>

- Mở xem lại: [Mở Javascript ES6](Javascript-ES6/readme.md)

***

## 🔶  Môi trường phát triển Reactjs

> 🔸 Node.js

- Node.js là 1 môi trường chạy mã javascript ở phía máy chủ.
- Nó cho phép chúng ta chạy javascript bên ngoài trình duyệt, giúp xây dựng ứng dụng web đa nền tảng.
- Node.js đi kèm với npm(Node Package Manager) hoặc yarn ( công cụ quản lý gói alternative)

> 🔸 Cài đặt Node.js

- Truy cập trang web chính thức của Node.js tại https://nodejs.org.
- Tải xuống phiên bản LTS (Long-Term Support) phù hợp với hệ điều hành của bạn.
- Chạy bộ cài đặt và hoàn thành quá trình cài đặt Node.js.

> 🔸 Kiểm tra cài đặt node.js và npm

- mở Terminal hoặc Command prompt trên máy tính của bạn
- gõ lệnh "node -v" để kiểm tra phiên bản Node.js đã được cài đặt
- gõ lệnh "npm -v" để kiểm tra phiên bản npm đã được cài đặt

> Nên dùng yarn để cho tốc độ cài đặt nhanh hơn