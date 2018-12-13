# Encryption-lock-using-AVR-microcontrollers
In this project, an encryption lock is simulated using AT mega 32, LCD, and keypad 3x4. 
1)	First the massage “enter pass” is displayed on the LCD.
2)	By pressing numbers from 0-9 on keypad, the massage is removed and the number is displayed on LCD. Then after 500 milliseconds, the number’s display changes to “*”.
3)	After entering a 4-digit password, by pressing “#” key on keypad, the entered password will be compared to the correct password which is “1396”. If the password you entered is “1396”, the massage: “correct” is displayed on LCD, otherwise, the massage “incorrect” is displayed and the system will be locked for 30 seconds. After 30 seconds, the massage “enter pass” is displayed again. 
4)	By holding “*” key for 1 second, the massage: “old pass?” is displayed. If the entered password is correct, the massage “new pass?” is displayed and receives a new 4-digit password from the user. If the old password is not entered correctly, the system returns to the first state of showing “enter pass” on LCD.
5)	Since it is probable that the user forget password, there is a possibility to reset the password by applying a 2-volt voltage difference between pins adc0 and adc1. This way the massage “reset pass” is displayed on LCD.

For interrupts, timer0 is used. 
Use the Proteus file (final project.pdsprj) for simulation of the project.
