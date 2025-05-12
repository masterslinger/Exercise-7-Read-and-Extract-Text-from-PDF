# Exercise-7-Read-and-Extract-Text-from-PDF

~~~
Name : M.JohnPall 
Reg.No : 212224040140 
~~~

## Aim
To create a UiPath workflow that reads and extracts text from a PDF file and saves the extracted content into a plain text file.

## Materials Required
UiPath Studio (Community or Enterprise Edition)
A sample PDF file (e.g., Sample.pdf)
Windows OS

UiPath PDF Activities Pack (Install via Manage Packages if not already installed)

## Procedure
Step 1: Create a New Process
Open UiPath Studio and create a new process named PDFTextExtractor.

Step 2: Install PDF Activities (If Needed)
Go to Manage Packages → Official → Search for UiPath.PDF.Activities.

Install and save.

Step 3: Add Variables
Create the following variables:

Name	Type	Default Value (if any)
pdfPath	String	"C:\Users\YourName\Documents\Sample.pdf"
textData	String	(leave blank)
textPath	String	"C:\Users\YourName\Documents\Output.txt"

Step 4: Add Read PDF Text Activity
Drag and drop the Read PDF Text activity from PDF Activities.

Set the properties:

FileName: pdfPath

Output: textData

Enable Preserve Formatting (optional)

Step 5: Write Text to File
Drag and drop Write Text File activity.

Set the properties:

FileName: textPath

Text: textData

Encoding: UTF-8 (optional)

## OUTPUT:
If your PDF contains:

~~~
This is a sample document.
It contains test content.
~~~
The text file Output.txt will have:

~~~
This is a sample document.
It contains test content.
~~~

![Screenshot 2025-05-11 214700](https://github.com/user-attachments/assets/994513ce-0a44-465d-afd9-72c453887f66)

![Screenshot 2025-05-11 214624](https://github.com/user-attachments/assets/b3e69a2e-662d-4046-8227-808c224dc511)

![Screenshot 2025-05-11 214640](https://github.com/user-attachments/assets/aca7833c-5e36-43e5-bbee-58e9c8fdcc30)

## Result:
The UiPath workflow successfully reads the content from a PDF file and writes it into a .txt file using built-in PDF and File activities.

