##PageSetup.GetEvenHeader
PageSetup method. Gets a script formatting the even header of an Excel file
## PageSetup.GetEvenHeader method
Gets a script formatting the even header of an Excel file.
```csharp
public string GetEvenHeader(int section)
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
public class PageSetupMethodGetEvenHeaderWithInt32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Enable different odd and even page headers/footers
PageSetup pageSetup = worksheet.PageSetup;
pageSetup.IsHFDiffOddEven = true;
// Set even page header
pageSetup.SetEvenHeader(0, "&CEven Page Header Center");
pageSetup.SetEvenHeader(1, "&LEven Page Header Left");
pageSetup.SetEvenHeader(2, "&REven Page Header Right");
// Get and print even page headers
Console.WriteLine("Even Header Center: " + pageSetup.GetEvenHeader(0));
Console.WriteLine("Even Header Left: " + pageSetup.GetEvenHeader(1));
Console.WriteLine("Even Header Right: " + pageSetup.GetEvenHeader(2));
// Save the workbook
workbook.Save("PageSetup_GetEvenHeaderDemo.xlsx");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
