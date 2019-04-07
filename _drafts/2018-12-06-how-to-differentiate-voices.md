---
layout: post
title:  "Giọng nói khác nhau như thế nào?"
# date:   2018-9-23 23:45:13 +0700
# subtitle: "The easiest way to get started with Tensorflow is using Eager Execution..."
author: AI Catchy Blog
background: '/img/posts/eager.jpeg'
tags: [tutorial, voice]
comments: true
---

Điều đầu tiên chúng ta cần xem xét là ***timbre*** (âm sắc). **Timbre** là thứ giúp chúng ta nhận diện được các loại nhạc cụ thậm chí khi chúng được chơi cùng một nốt nhạc (âm thanh cùng một nốt nhạc sẽ có cùng tần số)

**Frequency** (tần số) là thứ cho là đặc trưng của âm thanh. Khi có nhiều âm thanh khác tần số, chúng ta có thể dễ dàng nhận ra được sự khác biệt này. Vậy nếu hai âm thanh "khác nhau" có cùng tần số thì làm sao chúng ta có thể nhận ra sự khác biệt? Đó chính là nhờ **timbre**

**Vậy giọng nói của người thì sao?**

Giọng nói của người là sự kết hợp phức tạp của nhiều âm có tần số khác nhau với cường độ âm khác nhau. Những gì chúng ta nghe được là kết quả của một chùm đơn âm với cường độ khác nhau kết hợp lại.

Sự kết hợp này được tạo nên bởi các thành phần của giọng nói như hợp âm, lưỡi, họng, răng,...
Chính bởi sự khác nhau về cấu tạo vật lý của bộ tạo âm ở mỗi người nên mỗi người có một bộ "kết hợp âm" khác nhau, sự kết hợp này được gọi là **harmonics** (giai điệu). Đây cũng chính là **voice pattern** của mỗi người. Khi được nghe nhiều lần, não chúng ta sẽ tự xác định được **pattern** này và những biến đổi của nó trong quá trình nghe, tù đó chúng ta có thể xác định được ai đang nói mà không cần phải nhìn.

**Tại sao chúng ta có thể  nhận thấy được sự khác biệt về giọng nói thông qua loa/tai nghe?**
Khi giọng nói đi qua micro thu âm, chúng sẽ được chuyển đổi về các tín hiệu số , những tín hiệu số này cũng mang một *pattern* của người nói.