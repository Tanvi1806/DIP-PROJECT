# Number Plate Detection
 There are three programs or ‘.m’ files for this project.
 <br />
-**Template Creation** (template_creation.m)– This is used to call the saved images of alphanumerics and then save them as a new template in MATLAB memory.
 <br />
-**Letter Detection**(Letter_detection.m) – Reads the characters from the input image and find the highest matched corresponding alphanumeric.
 <br />
-**Plate Detection**(Plate_detection.m) – Process the image and then call the above two m-files to detect the number.
 <br />
 <br />
**Template Creation**
 <br />
First create a folder for the project (my folder name is Number Plate Detection) to save and store the files. We have stored the binary images of all the alphabets and numbers in the sub-folder named as ‘alpha'.
<br />
<br />
**Letter Detection**
<br />
Here we are creating the second code file named Letter_detection.m. Now, copy and paste the below code in that file and save the file in the project folder with name Letter_detection. 
<br/>
We have created a function named letter which gives us the alphanumeric output of the input image from class ‘alpha’ by using command ```readLetter()```.
<br/>We have resized the input image so it can be compared with the template’s images by using the command ```imresize(filename,size).``` Then for loop is used to correlates the input image with every image in the template to get the best match.
<br/>
<br/>
**Number Plate Detection**<br/>
The third and final code file named Plate_detection.m
<br/><br/>
```imread()``` – This command is used to open the image into the MATLAB from the target folder.
<br/><br/>
```rgb2gray()``` –This command is used to convert the RGB image into grayscale format.
<br/><br/>
```imbinarize()``` – This command is used to Binarize 2-D grayscale image or simply we can say it converts the image into black and white format.
<br/><br/>
```edge()``` – This command is used to detect the edges in the image, by using various methods like Roberts, Sobel, Prewitt and many others.
<br/><br/>
```regionprops()``` – This command is used to measure properties of image region.
<br/><br/>
```numel()``` – This command is used to calculate the number of array elements.
<br/><br/>
```imcrop()``` – This command is used to crop the image in the entered size.
<br/><br/>
```bwareaopen()``` – This command is used to remove small objects from binary image.
<br/><br/>
By using the above commands in the code, we are calling the input image and converting it into the grayscale. Then the grayscale is converted into the binary image, and the edge of the binary images is detected by the Prewitt method.
<br/>


