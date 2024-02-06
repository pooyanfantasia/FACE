# FACE RECOGNITION

# Wecome to face  recognition
>This is the final project of [CS50x](https://youtu.be/__Dvs-FdO38). This is a program to recognize people's faces. You can save people's faces with their names in the data storage area through the camera connected to the program. Then, whenever the person is in camera's field of view, the program will show the person's name in a green box

## Introduction
Click blow to see [video intro](https://youtu.be/VpiKutowMow):

## Explanation of program construction
To build this program, C# language has been used within the IDE of Visual Studio. In this program, we use the Haar Cascade libraries and EmguCV. 
When you save a person's face with its details, the program will see the face and recognize the name under which you have saved this face and show it to you.

## Construction Processes

### Creating a project 

1. open new project from the file menu and click on project and then Windows Forms app.
![](https://i.imgur.com/RwcEIpn.jpg)

2. from view tab click on Toolbox or ctrl + alt + x to open it.
![](https://i.imgur.com/mzFhZBh.jpg)

3. find picturebox from toolbox list or type picturebox and double click on it or drag it to design enviroment. add 2 pictureboxes
![](https://i.imgur.com/sKVUJxS.jpg)

4. add 2 labels from toolbox above of the pictureboxes. click on label and change the label name to Camera from properties tab and then from Font list find the text and type Camera and the second label to Captured.  
![](https://i.imgur.com/som5Q8L.jpg)

5. add another label blow the picture box and name it name. in front of the labe add a textbox from tollbox
1[](https://i.imgur.com/CUJRHlx.jpg)

6. add 3 buttons from toolbox to the form and name them Open Camera, Save Image and Detect Faces.
![](https://i.imgur.com/LHdiaFf.jpg)

### Adding and Using Library

7. Download the necessary files from the link blow
![](https://www.mediafire.com/folder/qp6jfwne9k9kn/faceRe-lib)

8. copy downloaded files in the directory of your project in my case C:\Users\name\source\repos\faceRecognition\bin\Debug

9. from solution explorer find References and right click and choose add references. click on brows and find the path of your project (setp 8 the coppied files) and choose FaceRecognition.dll
![](https://i.imgur.com/7sBPXFf.jpg)

10. add library by to the header of your pragram. right lick on the form and click on view code or press f7. type using FaceRecognition;
![](https://i.imgur.com/8oUXS6y.jpg)

11. creating a class with folowing codes FaceRec FaceRec faceRec = new FaceRec();


### Buttons Codes

## Open Camera button
Codes to activate the camera by pressing the Open Camera button

11. Double click on the Open Camera button to enter the codes.
 
## Save Imagese button 
Codes to save photo on memory. By the relevant code, after pressing the button, the user saves the desired name in the text box and shows a message like "saved successfull".

12. double click on Save Image to enter the codes. faceRec.Save_IMAGE(textBox1.Text);

## Detect FACE
Instance of a class related to face recognition and the property ‘isTrained’ is being used to indicate whether the model or system has been trained on the necessary data to perform its tasks

13. double click on Detect FACE to enter the codes. faceRec.isTrained = true;



### Installing EmguCV
Emgu CV is an open source C# library that allows you to add image processing functionality to your commercial software. Therefore, you can use Emgu CV to add image processing capabilities to the software you develop in the Microsoft Visual Studio environment.

12. from Soloution Explorer Right click on your program and choose Mange Nuget Packages... and search EmguCV in the search box and install it.
![](https://i.imgur.com/a9y0luj.jpg)


### Run The Program

Note: This is the desktop version of the program. If your computer does not have a webcam, you can use programs like Iruin webcam.
download link https://iriun.com/

13. After running the program, by pressing the open camera button, the program starts recording through the camera lens.
The program draws a green square as a frame by recognizing the face.

![](https://imgbox.com/j3R6UA4u)

14. When the program recognizes a person's face, you can specify a name for her in the name box and save it by pressing the Save Image button.
![](https://imgbox.com/lpMhXben)

15. When the program is monitoring the environment. By pressing the detect face button, if the person's name is already stored in the system, his name will be displayed.
![](https://imgbox.com/TYTr9ueH)

16. By saving the names of different faces, the program displays the saved faces in the capture section
![](https://imgbox.com/00q60Kgm)

17. Checking the same face in a different mode
![](https://imgbox.com/pYahcmYI)


Note: The program has different detection accuracy conditions and may encounter problems and errors in some cases.
