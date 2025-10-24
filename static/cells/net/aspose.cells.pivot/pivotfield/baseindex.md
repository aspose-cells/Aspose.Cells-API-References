##PivotField.BaseIndex
PivotField property. Represents the PivotField index in the base PivotFields
## PivotField.BaseIndex property
Represents the PivotField index in the base PivotFields.
```csharp
public int BaseIndex { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyBaseIndexDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
ws.Name = "PivotData";
// Sample data
ws.Cells["A1"].PutValue("Category");
ws.Cells["B1"].PutValue("Quarter");
ws.Cells["C1"].PutValue("Sales");
ws.Cells["A2"].PutValue("Electronics");
ws.Cells["A3"].PutValue("Electronics");
ws.Cells["A4"].PutValue("Clothing");
ws.Cells["A5"].PutValue("Clothing");
ws.Cells["B2"].PutValue("Q1");
ws.Cells["B3"].PutValue("Q2");
ws.Cells["B4"].PutValue("Q1");
ws.Cells["B5"].PutValue("Q2");
ws.Cells["C2"].PutValue(1000);
ws.Cells["C3"].PutValue(1200);
ws.Cells["C4"].PutValue(800);
ws.Cells["C5"].PutValue(900);
// Create pivot table - fixed by getting the PivotTable from the index
int pivotIndex = ws.PivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
PivotTable pt = ws.PivotTables[pivotIndex];
// Add row field
int rowIndex = pt.AddFieldToArea(PivotFieldType.Row, "Category");
PivotField rowField = pt.RowFields[rowIndex];
// Add column field (will be used as base field)
int colIndex = pt.AddFieldToArea(PivotFieldType.Column, "Quarter");
PivotField quarterField = pt.ColumnFields[colIndex];
// Add data field with normal calculation
int dataIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
PivotField dataField = pt.DataFields[dataIndex];
dataField.Function = ConsolidationFunction.Sum;
// Add second data field showing difference from previous quarter
int diffIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
PivotField diffField = pt.DataFields[diffIndex];
diffField.DisplayName = "QoQ Difference";
diffField.ShowValuesAs(
PivotFieldDataDisplayFormat.DifferenceFrom,
quarterField.BaseIndex,
PivotItemPositionType.Previous,
0);
// Calculate and save
wb.CalculateFormula();
wb.Save("PivotTableWithBaseIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
