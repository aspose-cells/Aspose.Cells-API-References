##Enum PivotItemPositionType
Aspose.Cells.Pivot.PivotItemPositionType enum. Represents the position type of the pivot base item in the base field when the ShowDataAs calculation is in use
## PivotItemPositionType enumeration
Represents the position type of the pivot base item in the base field when the ShowDataAs calculation is in use.
```csharp
public enum PivotItemPositionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Previous | `0` | Represents the previous pivot item in the PivotField. |
| Next | `1` | Represents the next pivot item in the PivotField. |
| Custom | `2` | Shows values as the different format based the index of pivot item in the PivotField. |
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
namespace AsposeCellsExamples
{
public class PivotItemPositionTypeDemo
{
public static void PivotItemPositionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Add a pivot table to the worksheet
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value
// Set the data display format to show values as difference from previous item
PivotField dataField = pivotTable.DataFields[0];
dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);
// Refresh and calculate the pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotItemPositionTypeExample.xlsx");
Console.WriteLine("Pivot table created and saved successfully.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
