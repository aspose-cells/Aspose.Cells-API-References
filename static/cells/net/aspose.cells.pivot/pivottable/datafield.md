##PivotTable.DataField
PivotTable property. Gets a PivotField object that represents all the data fields in a PivotTable. Readonly. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea method
## PivotTable.DataField property
Gets a [`PivotField`](../../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .
```csharp
public PivotField DataField { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyDataFieldDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B4"].Value = 3000;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Access and modify DataField properties
// Position is read-only, so we'll demonstrate other properties
pivotTable.DataField.DisplayName = "Total Sales";
pivotTable.DataField.NumberFormat = "#,##0";
// Save the workbook
workbook.Save("PivotTableDataFieldDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
