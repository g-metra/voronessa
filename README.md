# Voronessa Stream Timer
Easy to use, written in Python using Tkinter.  
Voronessa is a tool for counting down to the start of a broadcast.  
Download Installer for Windows (<ins>only x64</ins>) :

![1_logo](https://github.com/user-attachments/assets/2090e002-80b7-4461-8cdc-0660e32bf10a)

### Short description
+ Counts down from the setpoint (<ins>the minimum value is 1 minute, the maximum is 5940 minutes</ins>).
+ Cross-platform (<ins>tested on windows and popular linux distributions</ins>).

![3_window_linux](https://github.com/user-attachments/assets/b7766085-221b-48e6-a711-b3680327896c)

+ A style system, pre-defined styles, and the ability to customize your own.

![2_screen](https://github.com/user-attachments/assets/19f66789-82be-4cc5-ba6f-8cc06910436d)

### How to start using?
+ Install the binary build (<ins>only Windows x64</ins>).
+ Clone the repository and run <ins>main.py</ins> (<ins>Not all distributions include Python with the tkinter library. It must be installed separately.</ins>).

### Usage features
+ <ins>To close the countdown window, please use a double-click on the mouse or the Escape key.</ins>

### Using your own styles
**clock_pack directory map:**
```
(clock_pack) folder with styles
        |
      (CERAMIC, ASCII, etc.) folders defining the style
                  |
                (RED, WHITE, etc.) folders defining the style colors
                        |
                    (_0.png, 0.png, 1.png, etc.) images of the dial
```
+ The clock_pack folder contains folders that define styles.
+ The folder defining the style contains folders with colors of this style and the service file "!empty" which indicates that this style should be enabled when the program is launched.
+ + If the file "!empty" is missing or the name is changed, the style will be absent after the program is launched.
+ The folder defining the style color contains image files from 0.png to 9.png that define the dial and the _0.png file defining the separator, it also contains the "include" file that includes the style color when the program is launched.
+ + If the file "include" is missing or the name is changed, the color will be absent after the program is launched.

**example: clock_pack/CERAMIC/WHITE**
![4_directory_example](https://github.com/user-attachments/assets/48a99da4-dfd3-46f2-91ee-6435a00b7f3b)
+ The image file must be in the format .png with a resolution of 192x360.
+ Have an opaque black background to avoid display problems.
+ The file names must be in decimal from 0 to 9, and the file name must match the digit in the image. File name for separator _0.png
+ + _0.png = :
  + 0.png = 0
  + 1.png = 1
  + 2.png = 2
  + 3.png = 3
  + etc.  

**To sum up, to create your own style, you need:**
+ Create a folder in the clock_pack directory with the name of your style.
+ Place or create a "!empty" file without an extension in this style folder.
+ Create a folder with the name of the color in this style folder.
+ Place or create a "include" file without an extension in this color folder.
+ Place the pre-prepared images in the color-determining folder.
+ Done  
### One more thing
When creating the built-in styles, I used various fonts, all of them are "Free for commercial use" and "OFL". The list of fonts used when creating styles is in the file "fonts_used.txt ".
