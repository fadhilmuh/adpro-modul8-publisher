# How many data your publlsher program will send to the message broker in one run? 
Berdasarkan kode yang diberikan, setiap kali dijalankan, publisher akan mengirimkan lima pesan. Setiap kali fungsi p.publish_event dipanggil, satu pesan akan dikirim, di mana setiap pesan merupakan instance dari Pesan Acara User yang Dibuat dengan nilai user_id dan user_name yang berbeda.

# The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
Ketika URL "amqp://guest:guest@localhost:5672" digunakan di program subscriber dan publisher, ini berarti keduanya akan terhubung ke broker pesan yang sama menggunakan protokol AMQP. 
- "amqp://" menunjukkan bahwa koneksi menggunakan protokol AMQP.
- "guest:guest" adalah nama pengguna dan kata sandi default.
- "localhost:5672" menunjukkan bahwa broker pesan berjalan di mesin lokal pada port 5672.

Dengan menggunakan URL yang sama, baik program subscriber maupun publisher akan terhubung ke broker pesan yang sama, memfasilitasi pertukaran pesan antara keduanya. 

# Run RabbitMQ

![Run RabbitMQ](images/run_rabbitmq.png)