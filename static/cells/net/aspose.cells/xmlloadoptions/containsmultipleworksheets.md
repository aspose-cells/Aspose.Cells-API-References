##XmlLoadOptions.ContainsMultipleWorksheets
XmlLoadOptions property. Indicates whether importing xml as multiple worksheets
## XmlLoadOptions.ContainsMultipleWorksheets property
Indicates whether importing xml as multiple worksheets.
```csharp
public bool ContainsMultipleWorksheets { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XmlLoadOptionsPropertyContainsMultipleWorksheetsDemo
{
public static void Run()
{
// Create a sample Excel file with multiple worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets[0].Cells["A1"].PutValue("Data from Sheet1");
workbook.Worksheets[1].Cells["A1"].PutValue("Data from Sheet2");
workbook.Save("output.xlsx", SaveFormat.Xlsx);
// Save as XML with multiple worksheets
XmlSaveOptions saveOptions = new XmlSaveOptions();
saveOptions.SheetNameAsElementName = false;
workbook.Save("output.xml", saveOptions);
// Load the XML with ContainsMultipleWorksheets=true
XmlLoadOptions loadOptions = new XmlLoadOptions();
loadOptions.ContainsMultipleWorksheets = true;
Workbook loadedWorkbook = new Workbook("output.xml", loadOptions);
// Verify both worksheets were loaded
Console.WriteLine("Worksheet Count: " + loadedWorkbook.Worksheets.Count);
Console.WriteLine("Sheet1 Data: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
Console.WriteLine("Sheet2 Data: " + loadedWorkbook.Worksheets[1].Cells["A1"].StringValue);
}
}
}
```
### See Also
* class [XmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
