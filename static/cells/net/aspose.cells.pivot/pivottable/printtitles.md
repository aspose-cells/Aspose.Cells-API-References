##PivotTable.PrintTitles
PivotTable property. Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false
## PivotTable.PrintTitles property
Indicates whether the print titles for the worksheet are set based on the PivotTable report. The default value is false.
```csharp
public bool PrintTitles { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyPrintTitlesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(300);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Configure pivot table fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Demonstrate PrintTitles property
pivotTable.PrintTitles = true;
Console.WriteLine("PrintTitles set to: " + pivotTable.PrintTitles);
// Save the workbook
workbook.Save("PivotTablePrintTitlesDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
