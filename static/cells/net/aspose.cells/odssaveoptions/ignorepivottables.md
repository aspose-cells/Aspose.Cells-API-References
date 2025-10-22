##OdsSaveOptions.IgnorePivotTables
OdsSaveOptions property. Indicates whether saving pivot tables
## OdsSaveOptions.IgnorePivotTables property
Indicates whether saving pivot tables.
```csharp
public bool IgnorePivotTables { get; set; }
```
### Remarks
The pivot table feature of OpenOffice has fewer settings compared to Excel, so their results of pivot table have many differences. Sometimes it's better to ingore these pivot tables when saving .ods file.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B4"].PutValue(3000);
// Create a pivot table
PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Create OdsSaveOptions instance
OdsSaveOptions saveOptions = new OdsSaveOptions();
// Display current IgnorePivotTables value
Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);
// Set to ignore pivot tables when saving
saveOptions.IgnorePivotTables = true;
// Save with pivot tables ignored
workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);
// Set to include pivot tables when saving
saveOptions.IgnorePivotTables = false;
// Save with pivot tables included
workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
}
}
}
```
### See Also
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
