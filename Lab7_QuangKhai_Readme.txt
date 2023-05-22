Name: Quang Khai Le 
Class: EE 104


Lab 7: Yolov8 and Game dev 


Github link: https://github.com/blade199916/Lab7_Le_QuangKhai.git


Youtube link: https://youtu.be/wzOeZNPzQIM


1)We will use YAMOv5 to train the AI this time. 
You need to install YOLO5 file from https://github.com/ultralytics/yolov5
Python 3.10.8


Latest CUDA from https://developer.nvidia.com/cuda-downloads
PyTorch from https://pytorch.org/get-started/locally/
PyCOCOTools from https://github.com/philferriere/cocoapi.git 
Labelling Repo from https://github.com/ivangrov/ModifiedOpenLabelling
And pip install -r requirements.txt
After all the installation, download the images you want to train to C:\ModifiedOpenLabelling-main\images
Then run the ‘python run.py’ in cmd to label images with different names. 
Then Split the data into training and validation in cmd with commend line ‘python train_test_split.py’
Drag files in train folder to train folder in C:\yolov5\datasets\coco128, and same with the files in lable folder.
In the end, you could train your model in yolo cmd with the command line ‘python train.py --img 415 --batch 16 --epochs 100--data datasets/coco128_ee104.yaml --weight yolov5s.pt –cache’
Wait for the computer to finish the 100 epochs. And you will get a command line shows that the trained result is saved to ‘run\train\exp(number)
Then run ‘python detect.py --source 0 --weights C:\yolov5\runs\train\exp2\weights\best.pt’ but remember to change the number of the exp. And the result will show on your computer screen!
Hold off until the computer has completed 100 epochs. And you'll see on the command line that the trained result has been stored to "runtrainexp(number)" after running "python detect.py --source 0 --weights C:yolov5runstrainexp2weightsbest.pt". But don't forget to alter the exp number. Your computer screen will display the outcome as well!


  



  

  
  

Part 2: Balloon flight 


1. Balloon Game Information The Python software "Balloon Game" allows you to score points by steering a balloon while avoiding hazards like trees, buildings, and birds. The longer you manage to avoid striking obstacles, the greater your score will be in the game. The high scores will be updated if your score approaches or exceeds the five highest scores.




Start the Program
Follow these steps to execute the program:
On your PC, open a terminal window or command prompt.
Navigate to the program's save directory.
Enter the command as follows: balloons.py in Python
To play the game, according to the program's instructions.
necessary packages
Pygame