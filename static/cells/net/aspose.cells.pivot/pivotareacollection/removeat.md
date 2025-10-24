##PivotAreaCollection.RemoveAt
PivotAreaCollection method. Remove one pivot conditional formatted area setting
## PivotAreaCollection.RemoveAt method
Remove one pivot conditional formatted area setting.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotAreaCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(200);
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B4"].PutValue(300);
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Define cell areas to add to pivot areas
CellArea cellArea1 = new CellArea();
cellArea1.StartRow = 0;
cellArea1.StartColumn = 0;
cellArea1.EndRow = 2;
cellArea1.EndColumn = 1;
CellArea cellArea2 = new CellArea();
cellArea2.StartRow = 1;
cellArea2.StartColumn = 1;
cellArea2.EndRow = 3;
cellArea2.EndColumn = 2;
// Get pivot area collection by selecting the area
PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea1);
pivotAreas.Add(cellArea2);
try
{
// Display pivot areas before removal
Console.WriteLine("Pivot areas before removal:");
for (int i = 0; i < pivotAreas.Count; i++)
{
CellArea[] areas = pivotAreas[i].GetCellAreas();
foreach (CellArea ca in areas)
{
Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
}
}
// Call the RemoveAt method with Int32 parameter
pivotAreas.RemoveAt(0);
Console.WriteLine("\nPivot areas after removal:");
for (int i = 0; i < pivotAreas.Count; i++)
{
CellArea[] areas = pivotAreas[i].GetCellAreas();
foreach (CellArea ca in areas)
{
Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
}
}
}
catch (ArgumentOutOfRangeException ex)
{
Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
// Save the result
workbook.Save("PivotAreaCollectionMethodRemoveAtWithInt32Demo.xlsx");
}
}
}
```
### See Also
* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
