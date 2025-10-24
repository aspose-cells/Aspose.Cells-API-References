##XmlLoadOptions.StartCell
XmlLoadOptions property. Gets and sets the start cell
## XmlLoadOptions.StartCell property
Gets and sets the start cell.
```csharp
public string StartCell { get; set; }
```
### Remarks
Only works when the file is not speadsheetML or mapping xml to Excel.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlLoadOptionsPropertyStartCellDemo
{
public static void Run()
{
// Create an instance of XmlLoadOptions
XmlLoadOptions options = new XmlLoadOptions();
// Set the starting cell for XML data import
options.StartCell = "B2";
// Load an XML file into a Workbook using the specified options
Workbook workbook = new Workbook("input.xml", options);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Output the value from the start cell to demonstrate the property
Console.WriteLine("Value at start cell (B2): " + worksheet.Cells["B2"].Value);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
