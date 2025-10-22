##PivotField.RegionType
PivotField property. Specifies the region of the PivotTable that this field is displayed
## PivotField.RegionType property
Specifies the region of the PivotTable that this field is displayed.
```csharp
public PivotFieldType RegionType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFieldPropertyRegionTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Get the first pivot field
PivotField pivotField = pivotTable.RowFields[0];
// Display the current RegionType value
Console.WriteLine("Current RegionType value: " + pivotField.RegionType);
// Demonstrate how to use the RegionType property
if (pivotField.RegionType == PivotFieldType.Row)
{
Console.WriteLine("This pivot field is in the row area");
}
// Save the workbook
workbook.Save("PivotFieldRegionTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
