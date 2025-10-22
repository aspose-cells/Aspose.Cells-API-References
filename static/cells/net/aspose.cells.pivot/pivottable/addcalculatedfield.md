##PivotTable.AddCalculatedField
PivotTable method. Adds a calculated field to pivot field
## AddCalculatedField(string, string, bool) {#addcalculatedfield_1}
Adds a calculated field to pivot field.
```csharp
public void AddCalculatedField(string name, string formula, bool dragToDataArea)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |
| dragToDataArea | Boolean | True,drag this field to data area immediately |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodAddCalculatedFieldWithStringStringBooleanDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Sales";
cells["A2"].Value = "A";
cells["B2"].Value = 100;
cells["A3"].Value = "B";
cells["B3"].Value = 150;
cells["A4"].Value = "C";
cells["B4"].Value = 200;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add calculated field
pivotTable.AddCalculatedField("DoubleSales", "=Sales*2", true);
// Save the workbook
workbook.Save("PivotTableWithCalculatedField.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## AddCalculatedField(string, string) {#addcalculatedfield}
Adds a calculated field to pivot field and drag it to data area.
```csharp
public void AddCalculatedField(string name, string formula)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the calculated field |
| formula | String | The formula of the calculated field. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodAddCalculatedFieldWithStringStringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(15);
worksheet.Cells["B4"].PutValue(8);
worksheet.Cells["C1"].PutValue("Quantity");
worksheet.Cells["C2"].PutValue(5);
worksheet.Cells["C3"].PutValue(3);
worksheet.Cells["C4"].PutValue(10);
// Create pivot table collection
PivotTableCollection pivotTables = worksheet.PivotTables;
// Add pivot table and get its index
int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
// Get the pivot table object
PivotTable pivotTable = pivotTables[pivotIndex];
// Add fields to row area
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data fields
pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Add calculated field
pivotTable.AddCalculatedField("Total", "=Price*Quantity");
// Format the data field
pivotTable.DataFields["Total"].NumberFormat = "$#,##0.00";
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableWithCalculatedField.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
