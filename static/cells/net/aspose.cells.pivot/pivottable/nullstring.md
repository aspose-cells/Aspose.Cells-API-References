##PivotTable.NullString
PivotTable property. Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string
## PivotTable.NullString property
Gets the string displayed in cells that contain null values when the DisplayNullString property is true.The default value is an empty string.
```csharp
public string NullString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyNullStringDemo
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
cells["A2"].Value = "Apple";
cells["B2"].Value = 1000;
cells["A3"].Value = "Orange";
cells["B3"].Value = 2000;
cells["A4"].Value = "Banana";
cells["B4"].Value = 3000;
cells["A5"].Value = null; // Null value
cells["B5"].Value = 4000;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Set NullString property and display settings
pivotTable.NullString = "(null)";
pivotTable.DisplayNullString = true;
// Refresh pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableNullStringDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
