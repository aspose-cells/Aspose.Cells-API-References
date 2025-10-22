##PivotTable.SaveData
PivotTable property. Indicates whether data for the PivotTable report is saved with the workbook
## PivotTable.SaveData property
Indicates whether data for the PivotTable report is saved with the workbook.
```csharp
public bool SaveData { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertySaveDataDemo
{
public static void Run()
{
// Create a workbook with sample data
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
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Demonstrate SaveData property
Console.WriteLine("SaveData before setting: " + pivotTable.SaveData);
pivotTable.SaveData = false; // Disable saving pivot data with file
Console.WriteLine("SaveData after setting: " + pivotTable.SaveData);
// Save the workbook
workbook.Save("PivotTable_SaveData_Demo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
