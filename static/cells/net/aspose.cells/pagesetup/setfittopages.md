##PageSetup.SetFitToPages
PageSetup method. Sets the number of pages the worksheet will be scaled to when its printed
## PageSetup.SetFitToPages method
Sets the number of pages the worksheet will be scaled to when it's printed.
```csharp
public void SetFitToPages(int wide, int tall)
```
| Parameter | Type | Description |
| --- | --- | --- |
| wide | Int32 | Pages wide. |
| tall | Int32 | Pages tall. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupMethodSetFitToPagesWithInt32Int32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access the first worksheet's PageSetup
PageSetup setup = workbook.Worksheets[0].PageSetup;
// Set the fit to pages settings
setup.SetFitToPages(2, 3);
// Verify and output the settings
Console.WriteLine("IsPercentScale: " + setup.IsPercentScale);
Console.WriteLine("FitToPagesWide: " + setup.FitToPagesWide);
Console.WriteLine("FitToPagesTall: " + setup.FitToPagesTall);
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
