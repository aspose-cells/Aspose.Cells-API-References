##PivotTable.IsMultipleFieldFilters
PivotTable property. Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them
## PivotTable.IsMultipleFieldFilters property
Specifies a boolean value that indicates whether the fields of a PivotTable can have multiple filters set on them.
```csharp
[Obsolete("Use PivotTable.AllowMultipleFiltersPerField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsMultipleFieldFilters { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use PivotTable.AllowMultipleFiltersPerField property. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyIsMultipleFieldFiltersDemo
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
worksheet.Cells["B1"].PutValue("Category");
worksheet.Cells["B2"].PutValue("Fruit");
worksheet.Cells["B3"].PutValue("Fruit");
worksheet.Cells["B4"].PutValue("Fruit");
worksheet.Cells["C1"].PutValue("Sales");
worksheet.Cells["C2"].PutValue(1000);
worksheet.Cells["C3"].PutValue(2000);
worksheet.Cells["C4"].PutValue(3000);
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display the current value of IsMultipleFieldFilters
Console.WriteLine("Current IsMultipleFieldFilters value: " + pivotTable.IsMultipleFieldFilters);
// Set IsMultipleFieldFilters to true to allow multiple filters per field
pivotTable.IsMultipleFieldFilters = true;
Console.WriteLine("IsMultipleFieldFilters set to: " + pivotTable.IsMultipleFieldFilters);
// Refresh and calculate the pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTablePropertyIsMultipleFieldFiltersDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
