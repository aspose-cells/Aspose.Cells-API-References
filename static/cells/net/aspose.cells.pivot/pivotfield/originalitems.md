##PivotField.OriginalItems
PivotField property. Get the original base items
## PivotField.OriginalItems property
Get the original base items;
```csharp
public string[] OriginalItems { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyOriginalItemsDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("AsposeGroupedField2.xlsx");
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the first pivot table
PivotTable pivotTable = worksheet.PivotTables[0];
// Access the first row field
PivotField pivotField = pivotTable.RowFields[0];
// Display original items and grouped items
Console.WriteLine("Original Item[0]: " + pivotField.OriginalItems[0]);
Console.WriteLine("Grouped Item[0]: " + pivotField.Items[0]);
// Save the modified workbook
workbook.Save("PivotFieldOriginalItemsDemo_Output.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
