##PageSetup.Order
PageSetup property. Represents the order that Microsoft Excel uses to number pages when printing a large worksheet
## PageSetup.Order property
Represents the order that Microsoft Excel uses to number pages when printing a large worksheet.
```csharp
public PrintOrderType Order { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyOrderDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Set the print order to DownThenOver
sheet.PageSetup.Order = PrintOrderType.DownThenOver;
Console.WriteLine("Print order set to: " + sheet.PageSetup.Order);
// Save the workbook in different formats
workbook.Save("output_DownThenOver.xlsx", SaveFormat.Xlsx);
workbook.Save("output_DownThenOver.xls", SaveFormat.Excel97To2003);
// Change the print order to OverThenDown
sheet.PageSetup.Order = PrintOrderType.OverThenDown;
Console.WriteLine("Print order changed to: " + sheet.PageSetup.Order);
// Save again with different formats
workbook.Save("output_OverThenDown.xlsx", SaveFormat.Xlsx);
workbook.Save("output_OverThenDown.xls", SaveFormat.Excel97To2003);
}
}
}
```
### See Also
* enum [PrintOrderType](../../printordertype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
