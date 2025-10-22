##PageSetup.GetEvenFooter
PageSetup method. Gets a script formatting the even footer of an Excel file
## PageSetup.GetEvenFooter method
Gets a script formatting the even footer of an Excel file.
```csharp
public string GetEvenFooter(int section)
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
public class PageSetupMethodGetEvenFooterWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
PageSetup pageSetup = worksheet.PageSetup;
// Enable different headers/footers for odd and even pages
pageSetup.IsHFDiffOddEven = true;
// Set even footer
pageSetup.SetEvenFooter(0, "Even Page Footer");
// Get and display the even footer
string evenFooter = pageSetup.GetEvenFooter(0);
Console.WriteLine("Even Footer: " + evenFooter);
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
