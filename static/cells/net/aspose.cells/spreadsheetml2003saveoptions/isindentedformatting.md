##SpreadsheetML2003SaveOptions.IsIndentedFormatting
SpreadsheetML2003SaveOptions property. Causes child elements to be indented
## SpreadsheetML2003SaveOptions.IsIndentedFormatting property
Causes child elements to be indented.
```csharp
public bool IsIndentedFormatting { get; set; }
```
### Remarks
The default value is true. If the value is false, it will reduce the size of the xml file
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SpreadsheetML2003SaveOptionsPropertyIsIndentedFormattingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue(100);
// Configure save options with indented formatting
SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions
{
IsIndentedFormatting = true
};
// Save with indented XML formatting
workbook.Save("output_indented.xml", saveOptions);
// Save without indented formatting for comparison
saveOptions.IsIndentedFormatting = false;
workbook.Save("output_not_indented.xml", saveOptions);
}
}
}
```
### See Also
* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
