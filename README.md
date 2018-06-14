# LeitorXLSX
This project 

This application opens an xlsx file and prints the data using the C # platform, the prototype was built to test the C # features using a free package to manipulate files. The intention of the project is to build an api to control file features.

---------------
To use ClosedXML you must reference the DocumentFormat.OpenXml.dll:

DocumentFormat.OpenXml.dll for NET 4.0+

DocumentFormat.OpenXml.dll for NET 3.5
--------------

Im use for exemple save the document 

var workbook = new XLWorkbook();
var worksheet = workbook.Worksheets.Add("Sample Sheet");
worksheet.Cell("A1").Value = "Hello World!";
workbook.SaveAs("HelloWorld.xlsx");
ClosedXML makes it easier for developers to create Excel 2007+ (.xlsx, .xlsm, etc) files. It provides a nice object oriented way to manipulate the files (similar to VBA) without dealing with the hassles of XML Documents. It can be used by any .NET language like C# and Visual Basic (VB).

For more information see the wiki

Install ClosedXML via NuGet
If you want to include ClosedXML in your project, you can install it directly from NuGet

To install ClosedXML, run the following command in the Package Manager Console

PM> Install-Package ClosedXML
What can you do with this?
ClosedXML allows you to create Excel 2007+ (.xlsx, .xlsm, etc) files without the Excel application. The typical example is creating Excel reports on a web server.

If you've ever used the Microsoft Open XML Format SDK you know just how much code you have to write to get the same results as the following 4 lines of code.

var workbook = new XLWorkbook();
var worksheet = workbook.Worksheets.Add("Sample Sheet");
worksheet.Cell("A1").Value = "Hello World!";
workbook.SaveAs("HelloWorld.xlsx");
