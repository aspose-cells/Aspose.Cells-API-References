##Workbook.GetNamedStyle
Workbook method. Gets the named style in the style pool
## Workbook.GetNamedStyle method
Gets the named style in the style pool.
```csharp
public Style GetNamedStyle(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | name of the style |
### Return Value
named style, maybe null.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Data;
namespace AsposeCellsExamples
{
public class WorkbookMethodGetNamedStyleWithStringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add some named styles
Style style1 = workbook.CreateStyle();
style1.Name = "Number7";
style1.Custom = "#,##0.00";
Style style2 = workbook.CreateStyle();
style2.Name = "Center";
style2.HorizontalAlignment = TextAlignmentType.Center;
// Create sample data
DataTable dt = new DataTable();
dt.Columns.Add("ProductID", typeof(int));
dt.Columns.Add("ProductName", typeof(string));
dt.Columns.Add("Quantity", typeof(int));
dt.Columns.Add("UnitPrice", typeof(decimal));
dt.Columns.Add("Discount", typeof(float));
dt.Rows.Add(1, "Product A", 10, 19.99m, 0.1f);
dt.Rows.Add(2, "Product B", 5, 29.99m, 0.15f);
// Get worksheet and cells
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Get named styles
Style numberStyle = workbook.GetNamedStyle("Number7");
Style centerStyle = workbook.GetNamedStyle("Center");
// Apply styles to data
for(int i = 0; i < dt.Rows.Count; i++)
{
cells[i, 0].PutValue((int)dt.Rows[i]["ProductID"]);
cells[i, 0].SetStyle(centerStyle);
cells[i, 1].PutValue((string)dt.Rows[i]["ProductName"]);
cells[i, 3].PutValue((decimal)dt.Rows[i]["UnitPrice"]);
cells[i, 3].SetStyle(numberStyle);
}
// Save the workbook
workbook.Save("GetNamedStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
