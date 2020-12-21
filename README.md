# APLIKASI COLLISION DETECTION WITH MOUSE
Berdasarkan karakteristik *games* berdimensi 2D, untuk menangani *collision* yang berlebihan maka 
diperlukannya *event handling*. Kata *event* disini berarti suatu peristiwa yang 
dipicu oleh pengguna pasa suatu komponen GUI. Contoh *event handling* disini yaitu: 
- **Keyboard Handling**<br>
   Penyelesaian suatu *event* menggunakan *keyboard handling* ini digunakan pada aplikasi Space 
   Invader pada tugas sebelumnya. Untuk dapat melihat detailnya dapat dilihat pada link berikut: <br> 
   [Collision Detection](https://github.com/erzajanitra/CollisionDetection)
- **Mouse Handling**<br> 
   Berdasarkan link di atas, terdapat beberapa modifikasi agar dapat digunakan menggunakan *mouse handling*. 
   *Mouse Handling* sendiri merupakan sebuah metode dengan menggunakan *mouse* sebagai alat gerak pada 
   sebuah *event* yang diberikan oleh pengguna. Penjelasan cara kerja program dengan menggunakan *mouse
   handling* dapat dilihat di bawah ini. 

## Cara Kerja Program
### Board 
Pada *class* Board terdapat beberapa method yang diubah seperti: <br>
* Method ``initBoard``<br>
	Method ini bertugas untuk menginisialisasi Board Windows. Pada method ini terdapat beberapa modifikasi pada bagian: 



Perubahan dapat dilihat pada bagian `MouseHandler` dan `hideCursor` yang menggantikan fungsi `add(KeyListener)` dan `setFocusable` pada applikasi *Collision Detection* sebelumnya. Selanjutnya, membuat objek `MouseHandler` yang kemudian akan digunakan juga untuk menambah `MouseListener`.
<br> 
	
* Method ``hideCursor`` 
	Method ini berfungsi untuk menghilangkan *cursor* saat permainan berlangsung. <br> 
		
  	 
    

  
  
