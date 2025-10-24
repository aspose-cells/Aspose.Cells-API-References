##Class PivotFieldGroupSettings
Aspose.Cells.Pivot.PivotFieldGroupSettings class. Represents the group setting of pivot field
## PivotFieldGroupSettings class
Represents the group setting of pivot field.
```csharp
public class PivotFieldGroupSettings
```
## Constructors
| Name | Description |
| --- | --- |
| [PivotFieldGroupSettings](pivotfieldgroupsettings/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| virtual [Type](../../aspose.cells.pivot/pivotfieldgroupsettings/type/) { get; } | Gets the group type of pivot field. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldGroupSettingsDemo
{
public static void PivotFieldGroupSettingsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells[0, 0].Value = "Fruit";
worksheet.Cells[1, 0].Value = "Apple";
worksheet.Cells[2, 0].Value = "Banana";
worksheet.Cells[3, 0].Value = "Cherry";
worksheet.Cells[4, 0].Value = "Date";
worksheet.Cells[0, 1].Value = "Amount";
worksheet.Cells[1, 1].Value = 50;
worksheet.Cells[2, 1].Value = 60;
worksheet.Cells[3, 1].Value = 70;
worksheet.Cells[4, 1].Value = 80;
// Add a pivot table to the worksheet
int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount
// Access the row field
PivotField rowField = pivotTable.RowFields[0];
rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);
// Access the group settings of the row field
PivotFieldGroupSettings groupSettings = rowField.GroupSettings;
// Display the group type of the pivot field
Console.WriteLine("Group Type: " + groupSettings.Type);
// Save the workbook
workbook.Save("PivotFieldGroupSettingsExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
