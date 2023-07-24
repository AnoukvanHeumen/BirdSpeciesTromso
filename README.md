# Automated bird species classification from camera trap images based on YOLOv7

Make sure you have python and anaconda installed.

Clone this repository to your desktop and download the following file and paste it into the main folder.
https://www.dropbox.com/scl/fi/s6o9ncrcxano9ag727pvq/yolov7_bird_update.pt?rlkey=vky4tjzzwn4x71qydnbrj0u6n&dl=0 

You have to place the images you want to analyse in the data folder.

Then you open anaconda prompt and change the working directory using cd "INSERT YOUR DIRECTORY" (for example cd C:\Users\documents)

Create a conda environment by using the command “conda create -n yolov7-birds python=3.9”
And then "conda activate yolov7-birds"

Now you can run the following code to get the analysis started:
python detect.py --weights yolov7_bird_update.pt --conf 0.5 --img-size 640 --source data/ --no-trace --save-txt --save-conf


