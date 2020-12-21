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
         * Method ''initBoard''<br>
            Method ini bertugas untuk menginisialisasi Board Windows. Pada method ini terdapat beberapa modifikasi pada bagian: <br>
            
            ''' private void initBoard() {
    	
        setBackground(Color.BLACK);
        ingame = true; //menandain sedang dalam game
        
        //mouse handler
        MouseHandler handler = new MouseHandler();
		this.addMouseListener(handler);
		this.addMouseMotionListener(handler);
		//hideCursor agar ketika program di run, cursor mouse tidak terlihat
		this.hideCursor();
		
        //size board
        setPreferredSize(new Dimension(B_WIDTH, B_HEIGHT));
        //size spaceship
        spaceship = new SpaceShip(ICRAFT_X, ICRAFT_Y);

        initAliens();
        
        //delay waktu firing
        timer = new Timer(DELAY, this);
        timer.start();
    }
    '''
   Perubahan dapat dilihat pada bagian 'MouseHandler' dan 'hideCursor' yang menggantikan fungsi 'add(KeyListener)' dan 'setFocusable' pada applikasi *Collision Detection* sebelumnya.
   
   * Method ''hideCursor''<br>
     Pada fungsi ''hideCursor'' berfungsi untuk menghilangkan kursor saat permainan berlangsung. <br>
      ```hide
  public void hideCursor() {
	BufferedImage cursorImg = new BufferedImage(16, 16, BufferedImage.TYPE_INT_ARGB);
	Cursor blankCursor = Toolkit.getDefaultToolkit().createCustomCursor(
		cursorImg, new Point(0, 0), "blank cursor");
	this.setCursor(blankCursor);
  }
  ```
     
     
   ### Spaceship
   
## Class Diagram Collision Detection with Mouse

## Jalannya Program 
Untuk melihat jalannya program
