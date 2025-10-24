##Worksheet.AutoFilter
Worksheet property. Represents auto filter for the specified worksheet
## Worksheet.AutoFilter property
Represents auto filter for the specified worksheet.
```csharp
public AutoFilter AutoFilter { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyAutoFilterDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue("Electronics");
worksheet.Cells["A3"].PutValue("Shirt");
worksheet.Cells["B3"].PutValue("Clothing");
worksheet.Cells["A4"].PutValue("Phone");
worksheet.Cells["B4"].PutValue("Electronics");
worksheet.Cells["A5"].PutValue("Pants");
worksheet.Cells["B5"].PutValue("Clothing");
// Apply auto filter
worksheet.AutoFilter.Range = "A1:B5";
worksheet.AutoFilter.Filter(1, "Electronics");
// Refresh the filter
worksheet.AutoFilter.Refresh();
// Save the workbook
workbook.Save("AutoFilterDemo.xlsx");
}
}
}
```
### See Also
* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
