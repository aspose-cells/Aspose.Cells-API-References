##PivotField.Function
PivotField property. Represents the function used to summarize the PivotTable data field
## PivotField.Function property
Represents the function used to summarize the PivotTable data field.
```csharp
public ConsolidationFunction Function { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyFunctionDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add sample data
cells["A1"].Value = "Product";
cells["B1"].Value = "Sales";
cells["A2"].Value = "A";
cells["B2"].Value = 100;
cells["A3"].Value = "B";
cells["B3"].Value = 120;
cells["A4"].Value = "A";
cells["B4"].Value = 80;
cells["A5"].Value = "B";
cells["B5"].Value = 60;
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data field and set function to Max
int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
PivotField dataField = pivotTable.DataFields[fieldIndex];
dataField.Function = ConsolidationFunction.Max;
// Calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldFunctionDemo.xlsx");
}
}
}
```
### See Also
* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
