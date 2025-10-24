##ListColumn.SetDataStyle
ListColumn method. Sets the style of the data in this column of the table
## ListColumn.SetDataStyle method
Sets the style of the data in this column of the table.
```csharp
public void SetDataStyle(Style style)
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ListColumnMethodSetDataStyleWithStyleDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["A3"].PutValue("Data2");
// Create a list object (table)
int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[index];
// Get the style of first column
Style style = table.ListColumns[0].GetDataStyle();
// Modify the style
style.Pattern = BackgroundType.Solid;
style.BackgroundColor = System.Drawing.Color.Red;
// Apply the modified style to the column
table.ListColumns[0].SetDataStyle(style);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Style](../../../aspose.cells/style/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
