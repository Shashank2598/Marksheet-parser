# Marksheet-parser
Marksheet-parser is a tool for extracting structural information like Name, Marks Board etc. from Indian 10th/12th board Marksheets. It is written in python and uses tesseract OCR.

## Prerequsites
1) Windows 10 64 bit operating system
2) Marksheet-parser requires python 3.x
3) Google's Tesseract 4.00 (latest version) must be installed on your system.
4) Install  pycharm IDE and install the following python modules.
  * pytesseract
  * PIL(python Imaging Library) 
  * opencv-python
  * csv
  * scipy
  * difflib
  * numpy
5) Image specifications
  * Clear and good quality images.
  * Correctly rotated.
  * The structural information must be horizontally aligned with field names.
  * Brightness and contrast should be correct.
  * No shadows or perspective errors (Image examples are shown in Marksheet folder). 

## Running
Before executing the code

set path for tesseract in the code as below:
pytesseract.pytesseract.tesseract_cmd = 'C:\\Program Files (x86)\\Tesseract-OCR\\tesseract'

### Input:
All the marksheet images should be stored in Marksheets folder and input should be given in input.csv file.
Following are the input parameter-
StudentID, First Name, Last Name, MarksheetImageName

### Output:
Output is shown in output.csv file with the following fields added-
Board, Father's/Mother's/Guardian's Name, Roll No.,Date of Birth,School,(CGPA)/Result

The program performs good for CBSE marksheets.
