##PivotField.AutoShowField
PivotField property. Represents auto show field index. 1 means PivotField itself. It should be the index of the data fields
## PivotField.AutoShowField property
Represents auto show field index. -1 means PivotField itself. It should be the index of the data fields.
```csharp
public int AutoShowField { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyAutoShowFieldDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook();
// Add a worksheet and populate with sample data
Worksheet sheet = workbook.Worksheets[0];
Cells cells = sheet.Cells;
// Add sample data for pivot table
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
cells["A6"].Value = "Orange";
cells["B6"].Value = 10;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Configure AutoShow for the first pivot field
PivotField pivotField = pivotTable.RowFields[0];
pivotField.AutoShowCount = 2;
pivotField.AutoShowField = 1; // Index of data field (Quantity)
pivotField.IsAutoShow = true;
pivotField.IsAscendShow = true; // Equivalent to "Top" in AutoShowType
// Save the workbook
workbook.Save("PivotField_AutoShowField_Example.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
