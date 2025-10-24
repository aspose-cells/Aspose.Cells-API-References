##PivotField.Number
PivotField property. Represents the builtin display format of numbers and dates
## PivotField.Number property
Represents the built-in display format of numbers and dates.
```csharp
public int Number { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyNumberDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].PutValue("Date");
sheet.Cells["A2"].PutValue(new DateTime(2023, 1, 8));
sheet.Cells["A3"].PutValue(new DateTime(2023, 1, 15));
sheet.Cells["A4"].PutValue(new DateTime(2023, 1, 22));
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
PivotTable pivot = sheet.PivotTables[pivotIndex];
// Add date field to column area and set number format
int fieldIndex = pivot.AddFieldToArea(PivotFieldType.Column, 0);
PivotField field = pivot.ColumnFields[fieldIndex];
field.Number = 16; // d-mmm format
// Refresh and calculate pivot table
pivot.RefreshData();
pivot.CalculateData();
// Save the workbook
workbook.Save("PivotFieldNumberDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
