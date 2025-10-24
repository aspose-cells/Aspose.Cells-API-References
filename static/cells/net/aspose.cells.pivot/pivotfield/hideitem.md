##PivotField.HideItem
PivotField method. Sets whether the specific PivotItem in a data field is hidden
## HideItem(int, bool) {#hideitem}
Sets whether the specific PivotItem in a data field is hidden.
```csharp
public void HideItem(int index, bool isHidden)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | the index of the pivotItem in the pivotField. |
| isHidden | Boolean | whether the specific PivotItem is hidden |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodHideItemWithInt32BooleanDemo
{
public static void Run()
{
// Create a workbook with a sample pivot table
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Sample data for pivot table
sheet.Cells["A1"].PutValue("Product");
sheet.Cells["A2"].PutValue("PO-23-05");
sheet.Cells["A3"].PutValue("PO-23-06");
sheet.Cells["A4"].PutValue("PO-23-05");
sheet.Cells["A5"].PutValue("PO-23-07");
sheet.Cells["B1"].PutValue("Sales");
sheet.Cells["B2"].PutValue(1000);
sheet.Cells["B3"].PutValue(2000);
sheet.Cells["B4"].PutValue(1500);
sheet.Cells["B5"].PutValue(3000);
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get the pivot field
PivotField pivotField = pivotTable.RowFields[0];
// Hide items that are not "PO-23-05"
for (int i = 0; i < pivotField.ItemCount; i++)
{
pivotField.HideItem(i, pivotField.Items[i] != "PO-23-05");
}
// Calculate pivot table
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotFieldHideItemDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## HideItem(string, bool) {#hideitem_1}
Sets whether the specific PivotItem in a data field is hidden.
```csharp
public void HideItem(string itemValue, bool isHidden)
```
| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | String | the value of the pivotItem in the pivotField. |
| isHidden | Boolean | whether the specific PivotItem is hidden |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldMethodHideItemWithStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["A5"].Value = "Apple";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["B4"].Value = 20;
worksheet.Cells["B5"].Value = 5;
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Get the pivot field
PivotField pivotField = pivotTable.RowFields[0];
try
{
// Call the HideItem method with parameters (String, Boolean)
pivotField.HideItem("Apple", true);
Console.WriteLine("Method executed successfully with parameters (String, Boolean)");
Console.WriteLine("Apple items are now hidden in the pivot table");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing HideItem method: {ex.Message}");
}
// Save the result
workbook.Save("PivotFieldMethodHideItemWithStringBooleanDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
