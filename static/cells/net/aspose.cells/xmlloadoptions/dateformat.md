##XmlLoadOptions.DateFormat
XmlLoadOptions property. Gets and sets the format of date value
## XmlLoadOptions.DateFormat property
Gets and sets the format of date value.
```csharp
public string DateFormat { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlLoadOptionsPropertyDateFormatDemo
{
public static void Run()
{
// Create an instance of XmlLoadOptions
XmlLoadOptions options = new XmlLoadOptions();
// Set the date format for parsing dates from XML
options.DateFormat = "yyyy-MM-dd";
options.ConvertNumericOrDate = true;
// Load an XML file into a Workbook using the specified options
Workbook workbook = new Workbook("input.xml", options);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Display some cells to demonstrate date formatting
Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].Value);
Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].Value);
// Save the workbook to a new file
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
