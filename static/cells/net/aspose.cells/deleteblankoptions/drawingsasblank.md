##DeleteBlankOptions.DrawingsAsBlank
DeleteBlankOptions property. Whether drawing related objects such as picture shape chart... will be taken as blank. Default value is true
## DeleteBlankOptions.DrawingsAsBlank property
Whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true.
```csharp
public bool DrawingsAsBlank { get; set; }
```
### Remarks
When setting this property as false, all rows/columns covered by drawing objects will not be taken as blank and will not be deleted.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DeleteBlankOptionsPropertyDrawingsAsBlankDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data");
worksheet.Cells["B1"].PutValue("");
worksheet.Cells["B2"].PutValue("");
// Add a drawing object to test DrawingsAsBlank behavior
worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
// Delete blank columns with DrawingsAsBlank = false (preserves drawings)
worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });
Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
}
}
}
```
### See Also
* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
