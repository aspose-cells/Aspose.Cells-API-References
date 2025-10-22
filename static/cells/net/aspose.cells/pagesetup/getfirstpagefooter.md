##PageSetup.GetFirstPageFooter
PageSetup method. Gets a script formatting the first page footer of an Excel file
## PageSetup.GetFirstPageFooter method
Gets a script formatting the first page footer of an Excel file.
```csharp
public string GetFirstPageFooter(int section)
```
| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodGetFirstPageFooterWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set first page footer
worksheet.PageSetup.SetFirstPageFooter(1, "First Page Footer");
// Get and print first page footer
string footer = worksheet.PageSetup.GetFirstPageFooter(1);
Console.WriteLine("First Page Footer: " + footer);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
