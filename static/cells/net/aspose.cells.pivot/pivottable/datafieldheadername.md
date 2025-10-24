##PivotTable.DataFieldHeaderName
PivotTable property. Gets and sets the name of the value area field header in the PivotTable
## PivotTable.DataFieldHeaderName property
Gets and sets the name of the value area field header in the PivotTable.
```csharp
public string DataFieldHeaderName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyDataFieldHeaderNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Sales";
cells["A2"].Value = "Bike";
cells["B2"].Value = 1000;
cells["A3"].Value = "Car";
cells["B3"].Value = 2000;
cells["A4"].Value = "Bike";
cells["B4"].Value = 1500;
cells["A5"].Value = "Car";
cells["B5"].Value = 3000;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales
// Set custom data field header name
pivotTable.DataFieldHeaderName = "AsposeValues";
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableDataFieldHeaderNameDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
