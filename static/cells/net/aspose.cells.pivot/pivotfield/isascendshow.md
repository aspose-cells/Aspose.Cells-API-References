##PivotField.IsAscendShow
PivotField property. Indicates whether the specified PivotTable field is autoshown ascending
## PivotField.IsAscendShow property
Indicates whether the specified PivotTable field is autoshown ascending.
```csharp
public bool IsAscendShow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyIsAscendShowDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 150;
// Add pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
PivotField rowField = pivotTable.RowFields[0];
// Set IsAscendShow property
rowField.IsAscendShow = true;
Console.WriteLine("IsAscendShow (Row Field): " + rowField.IsAscendShow);
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
PivotField dataField = pivotTable.DataFields[0];
// Set IsAscendShow property
dataField.IsAscendShow = false;
Console.WriteLine("IsAscendShow (Data Field): " + dataField.IsAscendShow);
// Refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
