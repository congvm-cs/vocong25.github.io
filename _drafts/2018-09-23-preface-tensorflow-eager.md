---
layout: post
title:  "Tensorflow Eager cho người mới"
# date:   2018-9-23 23:45:13 +0700
subtitle: "The easiest way to get started with Tensorflow is using Eager Execution..."
author: Wu
background: '/img/posts/eager.jpeg'
tags: [tutorial, TF Eager]
comments: true
---
# __LỜI MỞ ĐẦU__

Vào ngày 30/3/2018, Google tổ chức hội nghị TensorFlow Dev Summit lần thứ hai ở Mountain View, California và thông báo về phiên bản chính thức Tensorflow 1.8. Hàng loạt những cập nhật đã được thêm vào phiên bản này. Đặc biệt, __Eager Execution Mode__ đã được giới thiệu và trình diễn từ 2017 nay chính thức thêm vào phiên bản mới này và Google khuyến nghị những người mới học TensorFlow nên sử dụng chế độ này.

> The easiest way to get started with Tensorflow is using Eager Execution.  
> --- https://www.tensorflow.org/get_started/

__Tại sao lại có Eager Execution Mode?__

Điểm lại một chút về hạn chế của __Graph Execution Mode__ trong TensorFlow, gồm khó tiếp cận với những người mới, khó khăn trong debugging, không linh hoạt và không thể kết hợp với Python trong coding. Những bất lợi này được đề cập rất nhiều trong giới lập trình ML/DL. Một số Deep Learning frameworks dựa vào __Dynamic Computational Graph__ (đồ thị tính toán động) như _PyTorch_ được phát triển và chiếm được nhiều sự ưu ái bởi tính dễ sử dụng và hiệu quả. Cụ thể hơn, framework này cực kì phổ biến trong giới nghiên cứu. Dù vậy, có rất nhiều sách lập trình, các bài hướng dẫn đều tập trung vào __Graph Execution Mode__, đây thực sự là một cơn ác mộng cho những người mới học. Hồi xưa mình cũng tự học Mode này, thực sự cực kì vất vả và cuối cùng mình chuyển qua Keras.Kể từ nay, Tensorflow cũng đã chính thức hỗ trợ __Eager Execution Mode__. 

Thực ra, Google cũng có nhiều bài hướng dẫn sử dụng [Eager Execution Mode](https://www.tensorflow.org/guide/eager). Tuy nhiên, mình không cảm thấy thực sự "ổn" cho những người mới bởi cấu trúc và thiếu đi những hướng dẫn "từng bước". Mình hy vọng bài đăng này của mình sẽ thay đổi được cách tiếp cận và tạo động lực cho những người mới học Machine Learning/Deep Learning bắt đầu dễ dàng hơn.

Những phần chính trong bài hướng dẫn này bao gồm:

- Phần hướng dẫn dựa chủ yếu tập trung vào Eager Mode trong TensorFlow. Tuy nhiên, mình cũng sẽ thêm vào các kiến thức của Graph Mode nếu cần thiết.
- Mình tập trung vào Coding, Modeling và ít tập trung vào những kiến thức nền tảng. Vậy nên, mình khuyên các bạn nên vừa học kiến thức nền tảng vừa học code để thực hành những ví dụ hoặc projects mà các bạn muốn làm.
- Càng ít càng tốt. Mình sẽ cố gắng cô động lại các kiến thức cần thiết để các bạn có thể hiểu dễ dàng hơn.

Mình thực hiện chuỗi bài này chủ yếu là để rèn luyện khả năng ngôn ngữ, tính logic trong tư duy, tự ôn luyện kiến thức và vì đam mê.

Bài hướng dẫn này được viết dựa trên [Jekyll](https://jekyllrb.com/), phần nội dung được tổng hợp ở nhiều nguồn khác nhau và được viết trên ngôn ngữ [Markdown](https://en.wikipedia.org/wiki/Markdown).

Ok! Hẹn gặp lại các bạn ở bài tiếp theo!