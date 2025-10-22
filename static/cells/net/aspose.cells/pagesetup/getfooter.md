##PageSetup.GetFooter
PageSetup method. Gets a script formatting the footer of an Excel file
## PageSetup.GetFooter method
Gets a script formatting the footer of an Excel file.
```csharp
public string GetFooter(int section)
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
public class PageSetupMethodGetFooterWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set different footer sections
worksheet.PageSetup.SetFooter(1, "odd");
worksheet.PageSetup.SetFirstPageFooter(1, "first");
worksheet.PageSetup.SetEvenFooter(1, "even");
// Get and display the footer sections
Console.WriteLine("First Page Footer: " + worksheet.PageSetup.GetFirstPageFooter(1));
Console.WriteLine("Even Page Footer: " + worksheet.PageSetup.GetEvenFooter(1));
Console.WriteLine("Odd Page Footer: " + worksheet.PageSetup.GetFooter(1));
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
