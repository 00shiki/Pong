# 1 - Pong

Kekurangan dari implementasi bola di tutorial ini adalah lajunya yang tidak stabil, dan bisa berbeda setiap kali bola mendapat gaya yang besarnya berbeda-beda saat bola mulai diluncurkan di set permainan baru . Modifikasilah kode tutorial ini supaya besar gaya yang diberikan kepada bola besarnya sama(kecepatan bola sama, kemanapun arahnya).

Petunjuk: lakukan implementasi di metode BallControl.PushBall(), dan ingat bahwa yang dibuat sama adalah besar gayanya, bukan gayanya itu sendiri.

## Solution

Setelah memperhatikan jalannya bola bergerak saya jadi tahu bahwa xInitialForce selalu konstan, sedangkan yInitialForce berubah-ubah. Hal itu mengakibatkan gaya pada vektor bola tidak konstan dan berubah-ubah. Oleh karena itu, saya mengubah xRandomInitialForce yang berubah berdasarkan perubahakan yRandomInitialForce. Saya menggunakan rumus vektor yang berbunyi ![rumus vektor](https://latex.codecogs.com/gif.latex?v%5E2%20%3D%20v_x%5E2%20&plus;%20v_y%5E2). Sehingga laju bola sekarang sudah konstan.
