##PivotTable.ErrorString
PivotTable property. Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string
## PivotTable.ErrorString property
Gets the string displayed in cells that contain errors when the DisplayErrorString property is true.The default value is an empty string.
```csharp
public string ErrorString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyErrorStringDemo
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
cells["B5"].Value = 1800;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Set ErrorString property
pivotTable.ErrorString = "Custom Error";
pivotTable.DisplayErrorString = true;
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Calculate data and refresh pivot table
pivotTable.CalculateData();
pivotTable.RefreshData();
// Save the workbook
workbook.Save("PivotTableErrorStringDemo.xlsx");
Console.WriteLine("PivotTable with ErrorString property set successfully.");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
