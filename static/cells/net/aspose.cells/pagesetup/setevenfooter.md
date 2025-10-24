##PageSetup.SetEvenFooter
PageSetup method. Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true
## PageSetup.SetEvenFooter method
Sets a script formatting the even page footer of an Excel file. Only effect in Excel 2007 when IsHFDiffOddEven is true.
```csharp
public void SetEvenFooter(int section, string footerScript)
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
public class PageSetupMethodSetEvenFooterWithInt32StringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
// Enable different headers/footers for first and even pages
pageSetup.IsHFDiffFirst = true;
pageSetup.IsHFDiffOddEven = true;
// Set different footer types
pageSetup.SetEvenFooter(0, "Even Page Footer");
pageSetup.SetFooter(0, "Odd Page Footer");
pageSetup.SetFirstPageFooter(0, "First Page Footer");
// Save the workbook
workbook.Save("PageSetup_SetEvenFooter_Example.xlsx");
Console.WriteLine("Workbook saved with even page footer set successfully.");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
