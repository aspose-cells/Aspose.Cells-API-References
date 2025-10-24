##AutoFilter.ShowFilterButton
AutoFilter property. Indicates whether the AutoFilter button for this column is visible
## AutoFilter.ShowFilterButton property
Indicates whether the AutoFilter button for this column is visible.
```csharp
public bool ShowFilterButton { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class AutoFilterPropertyShowFilterButtonDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create a list object/table
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
// Enable autofilter and show filter buttons
table.AutoFilter.ShowFilterButton = true;
// Save the workbook
workbook.Save("output_with_filter_buttons.xlsx");
// Hide filter buttons
table.AutoFilter.ShowFilterButton = false;
workbook.Save("output_without_filter_buttons.xlsx");
}
}
}
```
### See Also
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
