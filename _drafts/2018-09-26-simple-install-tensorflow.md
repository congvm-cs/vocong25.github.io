---
layout: post
title:  "Cài đặt Tensorflow"
# date:   2018-9-23 23:45:13 +0700
# subtitle: "The easiest way to get started with Tensorflow is using Eager Execution..."
author: Wu
background: '/img/posts/eager.jpeg'
tags: [tutorial, TF Eager]
comments: true
---

Bài hướng dẫn này sẽ có các phần như sau:

1. [Cài đặt Tensorflow](#setup)
2. [Chương trình đầu tiên](#program)

<a name="setup"></a>
# _1. Cài đặt Tensorflow_
Trước khi cài đặt Tensorflow, các bạn hãy cài đặt trước Python 3 phiên bản mới nhất từ trang https://www.python.org/ .

Mọi người có thể cài đặt Tensorflow từ trang web chính thức https://www.tensorflow.org/. Hiện nay, TensorFlow đã hỗ trợ rất nhiều ngôn ngữ như Python, Java và Go. Xuyên suốt các bài Tutorial này, mình sẽ sử dụng Python.

Một số chú ý nhỏ, các bạn nên cài đặt đúng môi trường theo các bước dưới đây:
1. Kiểm tra xem máy tính của bạn có NVIDIA graphic card không. Nếu có sẵn rồi thì bạn nên cài đặt Tensorflow phiên bản hỗ trợ GPU để tận dụng tối đa sức mạnh tính toán. Cụ thể hơn, để cài đúng CUDA, bạn nên truy cập vào trang [NVIDA official website](https://developer.nvidia.com/cuda-gpus/) để tìm phiên bản phù hợp. Nếu máy tính không hỗ trợ, thì bạn nên cài bản CPU.
2. Cài đặt môi trường Python. Mình khuyến nghị các bạn nên cài Anaconda. Đây là một thư viện khá đầy đủ bao gồm các thư viện phổ biến hiện nay như Numpy, Pandas,...

Nếu các bạn không thích cài đặt thêm thư viện mới thì các bạn có thể dùng [https://colab.research.google.com](https://colab.research.google.com) của Google và tạo một môi trường python để chạy chương trình bên dưới.

<a name="program"></a>
# _2. Chương trình đầu tiên_
Để kiểm tra xem liệu bạn đã cài đặt thành công hay chưa thì bạn hãy gõ dòng lệnh sau và chạy thử:

```python
import tensorflow as tf
tf.enable_eager_execution()

A = tf.constant([[1, 2], [3, 4]])
B = tf.constant([[5, 6], [7, 8]])
C = tf.matmul(A, B)

print(C)
```

Kết quả như sau:
```python
tf.Tensor([[19 22],[43 50]], shape=(2, 2), dtype=int32)
```
Nếu bạn chạy được đoạn script này có nghĩa là bạn đã cài đặt thành công Tensorflow rồi.


