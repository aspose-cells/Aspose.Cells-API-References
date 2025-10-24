##TableStyleElement.GetElementStyle
TableStyleElement method. Gets the element style
## TableStyleElement.GetElementStyle method
Gets the element style.
```csharp
public Style GetElementStyle()
```
### Return Value
Returns the [`Style`](../../../aspose.cells/style/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TableStyleElementMethodGetElementStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(2.5);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(1.8);
// Create a table
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[index];
// Get the table style from workbook's table style collection
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
TableStyle style = tableStyles[0];
table.TableStyleName = style.Name;
// Access the whole table style element
TableStyleElement element = style.TableStyleElements[TableStyleElementType.WholeTable];
// Get the element style
Style tableStyle = element.GetElementStyle();
// Modify the style properties
tableStyle.Font.Name = "Arial";
tableStyle.Font.Size = 12;
tableStyle.Font.IsBold = true;
tableStyle.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
tableStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
tableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
tableStyle.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
// Set the modified style back
element.SetElementStyle(tableStyle);
// Save the workbook
workbook.Save("TableStyleElementDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../../aspose.cells/style/)
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
