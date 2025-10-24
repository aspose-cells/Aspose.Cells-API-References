##PivotField.ShowCompact
PivotField property. Indicates whether display labels from the next field in the same column on the Pivot Table view
## PivotField.ShowCompact property
Indicates whether display labels from the next field in the same column on the Pivot Table view
```csharp
public bool ShowCompact { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyShowCompactDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Fruit");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Apple");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["A5"].PutValue("Orange");
worksheet.Cells["A6"].PutValue("Grape");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(150);
worksheet.Cells["B4"].PutValue(200);
worksheet.Cells["B5"].PutValue(250);
worksheet.Cells["B6"].PutValue(300);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A7", "A1:B6", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field and configure ShowCompact
int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
PivotField rowField = pivotTable.RowFields[fieldIndex];
rowField.ShowInOutlineForm = true;
rowField.ShowCompact = true;
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Calculate and refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldShowCompactDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
