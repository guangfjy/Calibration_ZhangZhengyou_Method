# Calibration_ZhangZhengyou_Method

Calibrate the camera with ZhangZhengyou method (in both distortion case and no distortion case)

本代码是知乎文章“相机标定之张正友标定法数学原理详解（含 python 源码）”的源代码。  
链接："https://zhuanlan.zhihu.com/p/94244568"

1. "calib_IR.py"对应"./pic/IR_camera_calib_img"文件夹，文件夹下图片含有畸变，  
   执行"calib_IR.py"得到到相机的内外参数与畸变参数，并对畸变图片做矫正，矫正图片保存在"./pic/save_dedistortion"文件夹下；

2. "calib_RGB.py"对应"./pic/RGB_camera_calib_img"文件夹，文件夹下图片不含畸变，  
   执行"calib_RGB.py"得到到相机的内外参数与畸变参数；

3. 棋盘格规格为 12 乘 9，格点长度 0.02m，由于 opencv 输入参数为内角点个数，所以输入参数为 11 乘 8。


相关配置：  
 win 10 / Ubuntu 16.04  
 python 3.5  
 opencv-contrib-python 3.4.2.16  
 opencv-python 3.4.2.16
