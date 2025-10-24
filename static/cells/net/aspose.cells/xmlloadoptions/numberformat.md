##XmlLoadOptions.NumberFormat
XmlLoadOptions property. Gets and sets the format of numeric value
## XmlLoadOptions.NumberFormat property
Gets and sets the format of numeric value.
```csharp
public string NumberFormat { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlLoadOptionsPropertyNumberFormatDemo
{
public static void Run()
{
// Create an instance of XmlLoadOptions
XmlLoadOptions options = new XmlLoadOptions();
// Set the NumberFormat property to display numbers with 2 decimal places
options.NumberFormat = "0.00";
// Load an XML file into a Workbook using the specified options
Workbook workbook = new Workbook("input.xml", options);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set some numeric values to demonstrate the number formatting
worksheet.Cells["A1"].PutValue(123);
worksheet.Cells["A2"].PutValue(45.678);
worksheet.Cells["A3"].PutValue(0.5);
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
