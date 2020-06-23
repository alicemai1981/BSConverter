# BSConverter
Convert bank statement in PDF to Excel spreadsheet 

This code uses Adobe acrobat Interapplication Communication API to convert pdf bank statements to excel spreadsheet  based on geometric location of each word.  see details: https://www.adobe.com/devnet/acrobat/interapplication_communication.html 

* To use this tool, open Visual Basic in excel and tick:  Tools -->References--> Acrobat 
* 1 file 1 account per run. make sure your pdf file is fully OCRed. 
* If your document contains fee breakdown blocks, select the "Ignore Fee Breakdown" option. This will slow down the code but will skip or wrap all the fee summary blocks so balance       calculation   will not be affected. 
* If "Comprehensive scan" is ticked, this code will work both on scanned hard copies and copies received eletronically. Otherwise this code only works on pdf files that happen to select words from left to right, top to bottom. (You can test if your file follows this order by selecting any word in the page and press Shift +Ctrl + -->).  Otherwise
* This code can not work with files with watermarks crossing the page. 
