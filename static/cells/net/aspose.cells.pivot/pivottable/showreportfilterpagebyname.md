##PivotTable.ShowReportFilterPageByName
PivotTable method. Show all the report filter pages according to PivotFields name the PivotField must be located in the PageFields
## PivotTable.ShowReportFilterPageByName method
Show all the report filter pages according to PivotField's name, the PivotField must be located in the PageFields.
```csharp
public void ShowReportFilterPageByName(string fieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | String | The name of PivotField |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodShowReportFilterPageByNameWithStringDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 20;
cells["A4"].Value = "Banana";
cells["B4"].Value = 15;
cells["A5"].Value = "Apple";
cells["B5"].Value = 5;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row and data fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Add page field
pivotTable.AddFieldToArea(PivotFieldType.Page, "Fruit");
pivotTable.PageFields[0].Name = "FruitFilter";
// Refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Show report filter pages by name
pivotTable.ShowReportFilterPageByName("FruitFilter");
// Save the workbook
workbook.Save("PivotTableShowReportFilterPageByNameDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
