##PivotTable.IsAutoFormat
PivotTable property. Indicates whether the PivotTable report is automatically formatted. Checkbox autoformat table  which is in pivottable option for Excel 2003
## PivotTable.IsAutoFormat property
Indicates whether the PivotTable report is automatically formatted. Checkbox "autoformat table " which is in pivottable option for Excel 2003
```csharp
public bool IsAutoFormat { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyIsAutoFormatDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B4"].PutValue(150);
// Add a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Set IsAutoFormat property
pivotTable.IsAutoFormat = true; // Enable auto formatting
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableIsAutoFormatDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
