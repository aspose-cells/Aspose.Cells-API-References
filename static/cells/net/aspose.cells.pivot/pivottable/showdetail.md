##PivotTable.ShowDetail
PivotTable method. Show the detail of one item in the data region to a new Table
## PivotTable.ShowDetail method
Show the detail of one item in the data region to a new Table.
```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Offset to the first data row in the data region. |
| columnOffset | Int32 | Offset to the first data column in the data region. |
| newSheet | Boolean | Show the detail to a new worksheet. |
| destRow | Int32 | The target row. |
| destColumn | Int32 | The target column. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Sport");
worksheet.Cells["A2"].PutValue("Tennis");
worksheet.Cells["A3"].PutValue("Basketball");
worksheet.Cells["A4"].PutValue("Tennis");
worksheet.Cells["B1"].PutValue("Score");
worksheet.Cells["B2"].PutValue(80);
worksheet.Cells["B3"].PutValue(90);
worksheet.Cells["B4"].PutValue(85);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");
// Show detail for specific cell
pivotTable.ShowDetail(1, 0, true, 0, 0);
// Save the workbook
workbook.Save("PivotTableShowDetailExample.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
