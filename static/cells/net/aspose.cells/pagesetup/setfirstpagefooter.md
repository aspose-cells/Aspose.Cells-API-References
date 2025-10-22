##PageSetup.SetFirstPageFooter
PageSetup method. Sets a script formatting the first page footer of an Excel file
## PageSetup.SetFirstPageFooter method
Sets a script formatting the first page footer of an Excel file.
```csharp
public void SetFirstPageFooter(int section, string footerScript)
```
| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |
| footerScript | String | Footer format script. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodSetFirstPageFooterWithInt32StringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get the PageSetup object
PageSetup pageSetup = worksheet.PageSetup;
// Set different headers/footers for first page
pageSetup.IsHFDiffFirst = true;
// Set first page footer with section index and text
pageSetup.SetFirstPageFooter(0, "First Page Footer Text");
// Save the workbook
workbook.Save("output.xlsx");
Console.WriteLine("First page footer set successfully.");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
