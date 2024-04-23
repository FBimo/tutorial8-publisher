# QnA
1. Berapa banyak data yang akan dikirimkan oleh publisher program ini ke _message broker_ dalam satu kali _run_?
    - Akan ada sebanyak lima data yang dikirmkan ke _message broker_ dalam satu kali _run_ karena terdapat lima _method_ `publish_event`.
2. Url “amqp://guest:guest@localhost:5672” sama saja dengan program subscriber, apa artinya?
    - Kedua _url_ sama saja karena keduanya mengirim _request_ ke server rabbitMQ. Hanya saja, _publisher_ mengirim pesan ke _queue_ sementara _subscriber_ akan mendapatkan data dari _queue_.
3. RabbitMQ Overview
![RabbitMQ-Overview](image.png)
4. Proses ketika _publisher_ mengirim lima data ke _queue_
![process-5-data-to-queue](image-1.png)
5. _Chart Monitoring_
Terjadi pelonjakan grafik karena _publisher_ telah melakukan _run_ beberapa kali.
![chart-monitoring](image-3.png)