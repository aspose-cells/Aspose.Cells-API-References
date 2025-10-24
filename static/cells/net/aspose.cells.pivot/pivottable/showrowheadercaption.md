##PivotTable.ShowRowHeaderCaption
PivotTable property. Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs
## PivotTable.ShowRowHeaderCaption property
Indicates whether row header caption is shown in the PivotTable report Indicates whether Display field captions and filter drop downs
```csharp
public bool ShowRowHeaderCaption { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyShowRowHeaderCaptionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and populate with sample data
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data for pivot table
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 15;
cells["A4"].Value = "Banana";
cells["B4"].Value = 20;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Demonstrate ShowRowHeaderCaption property
pivotTable.ShowRowHeaderCaption = true;
Console.WriteLine("Row Header Caption Visible: " + pivotTable.ShowRowHeaderCaption);
// Save the workbook
workbook.Save("PivotTableShowRowHeaderCaptionDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
