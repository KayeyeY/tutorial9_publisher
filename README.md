# Tutorial 9

### 1. How much data your publisher program will send to the message broker in one run?

Program publisher akan mengirim lima data ke message broker setiap kali dijalankan. Hal ini disebabkan karena fungsi ```main``` memanggil ```publish_event``` sebanyak lima kali, dan setiap pemanggilan ```publish_event``` mengirim satu objek ```UserCreatedEventMessage``` ke message broker.

### 2. Try to answer the following questions, and write the answer in the new file readme.md in your
repository.
Publisher dan subscriber sama-sama mengakses alamat ```amqp://guest:guest@localhost:5672```, yang berarti keduanya terhubung ke server AMQP yang sama. Dengan demikian, mereka berkomunikasi melalui message broker yang sama, sehingga pesan yang dikirim oleh publisher dapat diterima oleh subscriber yang terhubung ke server tersebut.

## Message Broker dengan RabbitMQ
### Running RabbitMQ as message broker
<img src="image/image1.png">

### Sending and Processing Event
<img src="image/image2.png">





