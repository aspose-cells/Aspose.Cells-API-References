##PivotTable.CopyStyle
PivotTable method. Copies named style from another pivot table
## PivotTable.CopyStyle method
Copies named style from another pivot table.
```csharp
public void CopyStyle(PivotTable pivotTable)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | PivotTable | Source pivot table. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodCopyStyleWithPivotTableDemo
{
public static void Run()
{
// Create source workbook with pivot table
Workbook sourceWorkbook = new Workbook();
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
// Add sample data
sourceSheet.Cells["A1"].PutValue("Product");
sourceSheet.Cells["B1"].PutValue("Sales");
sourceSheet.Cells["A2"].PutValue("A");
sourceSheet.Cells["B2"].PutValue(100);
sourceSheet.Cells["A3"].PutValue("B");
sourceSheet.Cells["B3"].PutValue(200);
// Create source pivot table (explicitly get the pivot table object)
PivotTable sourcePivotTable = sourceSheet.PivotTables[sourceSheet.PivotTables.Add("PivotTable1", "A1:B3", "C3")];
sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Apply style to source pivot table
sourcePivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
// Create destination workbook with pivot table
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets[0];
// Add same data structure
destSheet.Cells["A1"].PutValue("Product");
destSheet.Cells["B1"].PutValue("Sales");
destSheet.Cells["A2"].PutValue("A");
destSheet.Cells["B2"].PutValue(150);
destSheet.Cells["A3"].PutValue("B");
destSheet.Cells["B3"].PutValue(250);
// Create destination pivot table (explicitly get the pivot table object)
PivotTable destPivotTable = destSheet.PivotTables[destSheet.PivotTables.Add("PivotTable2", "A1:B3", "C3")];
destPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
destPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Copy style from source to destination pivot table
destPivotTable.CopyStyle(sourcePivotTable);
// Save the result
destWorkbook.Save("PivotTableStyleCopied.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
