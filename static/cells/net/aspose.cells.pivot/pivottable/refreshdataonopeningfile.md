##PivotTable.RefreshDataOnOpeningFile
PivotTable property. Indicates whether Refresh Data when Opening File
## PivotTable.RefreshDataOnOpeningFile property
Indicates whether Refresh Data when Opening File.
```csharp
public bool RefreshDataOnOpeningFile { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyRefreshDataOnOpeningFileDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = worksheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Sales";
cells["A2"].Value = "Apple";
cells["B2"].Value = 1000;
cells["A3"].Value = "Banana";
cells["B3"].Value = 2000;
cells["A4"].Value = "Orange";
cells["B4"].Value = 3000;
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Set RefreshDataOnOpeningFile property
pivotTable.RefreshDataOnOpeningFile = false;
// Save the workbook
workbook.Save("PivotTableRefreshDataOnOpeningFileDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
