##PivotFieldCollection.Add
PivotFieldCollection method. Adds a PivotField Object to the specific type PivotFields
## PivotFieldCollection.Add method
Adds a PivotField Object to the specific type PivotFields.
```csharp
public int Add(PivotField pivotField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | a PivotField Object. |
### Return Value
the index of the PivotField Object in this PivotFields.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldCollectionMethodAddWithPivotFieldDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("sample_pivot_table.xlsx");
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the first pivot table
PivotTable pivotTable = worksheet.PivotTables[0];
// Refresh pivot table data
pivotTable.RefreshData();
// Add data field to column fields area using Add method
pivotTable.ColumnFields.Add(pivotTable.DataField);
// Calculate pivot table data
pivotTable.CalculateData();
// Save the workbook
workbook.Save("output_pivot_table.xlsx");
}
}
}
```
### See Also
* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
