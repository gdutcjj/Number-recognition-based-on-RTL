# Number-recognition-based-on-RTL
A number recognition system bulitd by RTL，and few IP. Can be used in Xilinx FPGA.
tips:
1)There are detailed comments in the code。Download at ease
2)Using this project requires a Xilinx FPGA development board, ov7725 camera and HDMI display.

In the system, the OV7725 camera is first used to extract real-time image input classifier for recognition. The input camera image is cut into an image size of 320*240, then converted into a grayscale, and finally scaled into a grayscale size of 28*28 (the specific method is to use 8*8 matrix to cut the image, Add the 64 pixels within each 8*8 matrix and assign them as new pixels) into the LeNet network. LeNet network parameters are stored in the database (RAM)....Specific reports will be updated when available....


![image](https://user-images.githubusercontent.com/103297071/229667419-b0abf60c-bf52-4a9b-b745-e3fdb0076378.png)
![image](https://user-images.githubusercontent.com/103297071/229667440-4ddf5382-3e51-417d-863e-0cfef8b4baba.png)

x7c325t Resource usage after deployment

![image](https://user-images.githubusercontent.com/103297071/229667579-da50c222-acac-41ca-abca-708a809a1419.png)
![image](https://user-images.githubusercontent.com/103297071/229667604-d12b512a-38c5-4865-bac6-a96e1f211de7.png)

test result

Letnet identification network section references the following design

https://github.com/suisuisi/FPGAandCNN/blob/main/images/Neura
