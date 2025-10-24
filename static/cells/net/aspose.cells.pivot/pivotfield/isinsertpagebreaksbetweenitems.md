##PivotField.IsInsertPageBreaksBetweenItems
PivotField property. Indicates whether inserting page breaks after each item. The default value is false
## PivotField.IsInsertPageBreaksBetweenItems property
Indicates whether inserting page breaks after each item. The default value is false.
```csharp
public bool IsInsertPageBreaksBetweenItems { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyIsInsertPageBreaksBetweenItemsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
for (int i = 2; i <= 7; i++)
{
worksheet.Cells["A" + i].PutValue("Category " + (i % 3 + 1));
worksheet.Cells["B" + i].PutValue(i * 100);
}
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Check page count before setting property
SheetRender render1 = new SheetRender(worksheet, new ImageOrPrintOptions());
Console.WriteLine("Page count before: " + render1.PageCount);
// Set IsInsertPageBreaksBetweenItems property
PivotField field = pivotTable.RowFields[0];
field.IsInsertPageBreaksBetweenItems = true;
pivotTable.RefreshData();
pivotTable.CalculateData();
// Check page count after setting property
SheetRender render2 = new SheetRender(worksheet, new ImageOrPrintOptions());
Console.WriteLine("Page count after: " + render2.PageCount);
// Save the workbook
workbook.Save("PivotFieldIsInsertPageBreaksBetweenItemsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
