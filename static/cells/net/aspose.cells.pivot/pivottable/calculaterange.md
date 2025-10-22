##PivotTable.CalculateRange
PivotTable method. Calculates pivottables range
## PivotTable.CalculateRange method
Calculates pivottable's range.
```csharp
public void CalculateRange()
```
### Remarks
If this method is not been called,maybe the pivottable range is not corrected.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodCalculateRangeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data to the first worksheet
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Cells["A1"].PutValue("Product");
dataSheet.Cells["B1"].PutValue("Sales");
dataSheet.Cells["A2"].PutValue("Apple");
dataSheet.Cells["B2"].PutValue(1000);
dataSheet.Cells["A3"].PutValue("Banana");
dataSheet.Cells["B3"].PutValue(2000);
dataSheet.Cells["A4"].PutValue("Orange");
dataSheet.Cells["B4"].PutValue(3000);
// Add a pivot table
Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
int pivotIndex = pivotSheet.PivotTables.Add("A1", "A1:B4", "PivotTable1");
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
// Add row and data fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Calculate range and refresh data
pivotTable.CalculateRange();
pivotTable.CalculateData();
pivotTable.RefreshData();
// Save the workbook
workbook.Save("PivotTableCalculateRangeDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
