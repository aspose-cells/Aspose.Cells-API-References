##OdsLoadOptions.RefreshPivotTables
OdsLoadOptions property. Indicates whether refresh pivot tables when loading file
## OdsLoadOptions.RefreshPivotTables property
Indicates whether refresh pivot tables when loading file.
```csharp
public bool RefreshPivotTables { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class OdsLoadOptionsPropertyRefreshPivotTablesDemo
{
public static void Run()
{
// Create a sample workbook with pivot table
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("Fruit");
sheet.Cells["A3"].PutValue("Fruit");
sheet.Cells["A4"].PutValue("Vegetable");
sheet.Cells["B1"].PutValue("Item");
sheet.Cells["B2"].PutValue("Apple");
sheet.Cells["B3"].PutValue("Orange");
sheet.Cells["B4"].PutValue("Carrot");
sheet.Cells["C1"].PutValue("Price");
sheet.Cells["C2"].PutValue(2.5);
sheet.Cells["C3"].PutValue(3.0);
sheet.Cells["C4"].PutValue(1.5);
// Create pivot table
int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
// Save as ODS
string odsPath = "output.ods";
wb.Save(odsPath, SaveFormat.Ods);
// Load with RefreshPivotTables enabled
OdsLoadOptions loadOptions = new OdsLoadOptions();
loadOptions.RefreshPivotTables = true;
Workbook wb2 = new Workbook(odsPath, loadOptions);
// Verify pivot table was refreshed
Console.WriteLine("Pivot table refreshed: " + wb2.Worksheets[0].PivotTables[0].RefreshDataFlag);
}
}
}
```
### See Also
* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
