##SubtotalSetting.TotalList
SubtotalSetting property. An array of zerobased field offsets indicating the fields to which the subtotals are added
## SubtotalSetting.TotalList property
An array of zero-based field offsets, indicating the fields to which the subtotals are added.
```csharp
public int[] TotalList { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SubtotalSettingPropertyTotalListDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Sample data setup
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["A5"].PutValue("B");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
worksheet.Cells["B5"].PutValue(40);
// Create and apply subtotal
CellArea area = CellArea.CreateCellArea("A1", "B5");
worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 }, true, true, true);
// Retrieve subtotal setting to demonstrate TotalList usage
SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
Console.WriteLine("TotalList contains column index: " + subtotal.TotalList[0]);
// Save the workbook
workbook.Save("SubtotalDemo.xlsx");
}
}
}
```
### See Also
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
