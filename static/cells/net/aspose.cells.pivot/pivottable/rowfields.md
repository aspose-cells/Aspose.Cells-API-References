##PivotTable.RowFields
PivotTable property. Returns a PivotFields object that are currently shown as row fields
## PivotTable.RowFields property
Returns a PivotFields object that are currently shown as row fields.
```csharp
public PivotFieldCollection RowFields { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyRowFieldsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Region";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Bike";
cells["B2"].Value = "North";
cells["C2"].Value = 1000;
cells["A3"].Value = "Bike";
cells["B3"].Value = "South";
cells["C3"].Value = 800;
cells["A4"].Value = "Car";
cells["B4"].Value = "North";
cells["C4"].Value = 1500;
cells["A5"].Value = "Car";
cells["B5"].Value = "South";
cells["C5"].Value = 1200;
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add row fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Demonstrate RowFields property
Console.WriteLine("Row Fields Count: " + pivotTable.RowFields.Count);
Console.WriteLine("First Row Field Name: " + pivotTable.RowFields[0].Name);
Console.WriteLine("Second Row Field Name: " + pivotTable.RowFields[1].Name);
// Save the workbook
workbook.Save("PivotTableRowFieldsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
