##PivotTable.DisplayErrorString
PivotTable property. Indicates whether the PivotTable report displays a custom string in cells that contain errors
## PivotTable.DisplayErrorString property
Indicates whether the PivotTable report displays a custom string in cells that contain errors.
```csharp
public bool DisplayErrorString { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyDisplayErrorStringDemo
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
cells["B5"].Value = 2500;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Set DisplayErrorString property and demonstrate its usage
pivotTable.DisplayErrorString = true;
pivotTable.ErrorString = "Custom Error";
// Calculate data to show the effect
pivotTable.CalculateData();
Console.WriteLine("DisplayErrorString is set to: " + pivotTable.DisplayErrorString);
Console.WriteLine("ErrorString is set to: " + pivotTable.ErrorString);
// Save the workbook
workbook.Save("PivotTablePropertyDisplayErrorStringDemo_out.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
