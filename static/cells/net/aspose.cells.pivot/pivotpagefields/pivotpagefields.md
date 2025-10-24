##PivotPageFields.PivotPageFields
PivotPageFields constructor. Represents the pivot page field items
## PivotPageFields constructor
Represents the pivot page field items.
```csharp
public PivotPageFields()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotPageFieldsMethodSharpctorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Region");
worksheet.Cells["C1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue("East");
worksheet.Cells["C2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Item2");
worksheet.Cells["B3"].PutValue("West");
worksheet.Cells["C3"].PutValue(2000);
// Create pivot page fields using constructor
PivotPageFields pageFields = new PivotPageFields();
// Add page fields
string[] items = { "Item1", "Item2" };
pageFields.AddPageField(items);
// Add identification
int[] itemIndexes = { 0, 1 };
pageFields.AddIdentify(0, itemIndexes);
// Add pivot table with correct parameters
PivotTableCollection pivotTables = worksheet.PivotTables;
string sourceData = "A1:C3";
int index = pivotTables.Add(sourceData, "E5", "PivotTable1");
// Save the workbook
workbook.Save("PivotPageFieldsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
