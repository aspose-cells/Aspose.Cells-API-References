##PivotTable.EnableFieldList
PivotTable property. Indicates whether the field list for the PivotTable is available on the view of Excel
## PivotTable.EnableFieldList property
Indicates whether the field list for the PivotTable is available on the view of Excel.
```csharp
public bool EnableFieldList { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyEnableFieldListDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 15;
cells["A4"].Value = "Banana";
cells["B4"].Value = 20;
// Add a pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Set EnableFieldList property
pivotTable.EnableFieldList = false;
// Save the workbook
workbook.Save("PivotTable_EnableFieldList_Demo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
