---
layout: post
title:  "Vấn đề của bài toán tổng hợp giọng nói - P1"
# date:   2018-9-23 23:45:13 +0700
# subtitle: "The easiest way to get started with Tensorflow is using Eager Execution..."
author: Wu
background: '/img/posts/text-to-speech.jpg'
tags: [tutorial, TTS]
comments: true
---

# TỔNG HỢP GIỌNG NÓI

Trong phần này chúng ta sẽ cùng bàn luận về  tổng hợp giọng nói (TTS).

Trong TTS, đầu vào là chữ viết và đầu ra là giọng nói. Ngôn ngữ là cái gì đó rất độc đáo. Chúng ta có thể coi chữ viết là một loại tín hiệu, giống như giọng nói.

**Đọc** là một quá trình giải mã tín hiệu chữ thành thông điệp (message), sau đó **Hiểu** để tiếp thu ý nghĩa của thông điệp. Mình xin nhấn mạnh rằng, không có sự phân biệt nào giữa tín hiệu và hình thức trong quá trình viết. Chúng ta chỉ quan tâm tín hiệu này đơn tuần chỉ là "chữ trên trang giấy". Một sự phân biệt đơn giản hơn giữa câu chữ và phát âm là chữ viết là sự giản lượt của ngôn ngữ.

Với một cái nhìn có "định hướng", chúng ta cùng xem xét các hình thái của ngôn ngữ một cách rõ ràng, hơi chút trừu tượng.

Quá trình đọc lớn (Read out loud) là quá trình chuyển hóa chữ viết thành một dạng khác, đó là giọng nói. Chúng ta sẽ cùng phân tích một số câu hỏi:

- Tại sao chúng ta phải giải mã ngôn ngữ viết?
- Thông điệp mà chúng ta xuất trích ra từ tín hiệu dạng chữ viết có chứa đầy đủ thông để tái tạo lại giọng nói?
- Khi một người đọc lớn, có mối quan hệ giữa tác giả, người đọc và người nghe?
- Người nghe muốn gì việc tổng hợp giọng nói?
  
Chúng ta sẽ cùng chờ xem ở các phần tiếp theo để cùng trả lời các câu hỏi trên nhé.
