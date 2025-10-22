##PivotTable.DisplayNullString
PivotTable property. Indicates whether the PivotTable report displays a custom string if the value is null
## PivotTable.DisplayNullString property
Indicates whether the PivotTable report displays a custom string if the value is null.
```csharp
public bool DisplayNullString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyDisplayNullStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and populate with sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue(null);
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["B4"].PutValue(null);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Set DisplayNullString property and custom null string
pivotTable.DisplayNullString = true;
pivotTable.NullString = "N/A";
// Calculate data and refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableDisplayNullStringDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
