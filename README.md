# -target-STM32F401-drivers-SPI-FD
This project uses STM32CubeIDE and it's a program created to practice my C habilities during the course 'Mastering Microcontroller and Embedded Driver Development' from FastBit Embedded Brain Academy. I am using a NUCLEO-F401RE board.

##

In the library drive .c we implemented the SPI_ReceiveData API.

![image](https://user-images.githubusercontent.com/58916022/209197143-2dd80fa3-bbd3-4b91-baa2-a00f065a0882.png)

Now we are configuring the MISO pin:

![image](https://user-images.githubusercontent.com/58916022/209196966-456c6d62-9e00-43d2-9044-22dfbbbb4a4b.png)

We add some command codes:

![image](https://user-images.githubusercontent.com/58916022/209197734-6895337d-b919-4edc-ac29-455731523dcf.png)

		// JUST FIRST PART WILL BE IMPLEMENTED AND TESTED LATER
		// Lesson learned: SPI is a shift register
		// Every byte sent, 1 dummy byte read
		// Every byte that need to be read, 1 dummy byte has to be send
