##LoadOptions.IgnoreNotPrinted
LoadOptions property. Ignore the data which are not printed if directly printing the file
## LoadOptions.IgnoreNotPrinted property
Ignore the data which are not printed if directly printing the file
```csharp
public bool IgnoreNotPrinted { get; set; }
```
### Remarks
Only for xlsx file.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyIgnoreNotPrintedDemo
{
public static void Run()
{
// Create HTML load options and set IgnoreNotPrinted
HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
loadOptions.IgnoreNotPrinted = true;
loadOptions.AutoFitColsAndRows = true;
// Load HTML file with the specified options
Workbook workbook = new Workbook("example.html", loadOptions);
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate the effect of IgnoreNotPrinted by checking cell styles
Console.WriteLine("B3 Cell Color: " + worksheet.Cells["B3"].GetStyle().ForegroundColor);
Console.WriteLine("B4 Cell Color: " + worksheet.Cells["B4"].GetStyle().ForegroundColor);
Console.WriteLine("B5 Cell Color: " + worksheet.Cells["B5"].GetStyle().ForegroundColor);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
