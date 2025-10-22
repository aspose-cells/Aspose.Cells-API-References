##TableStyle.TableStyleElements
TableStyle property. Gets all elements of the table style
## TableStyle.TableStyleElements property
Gets all elements of the table style.
```csharp
public TableStyleElementCollection TableStyleElements { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TableStylePropertyTableStyleElementsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for the table
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create a table
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[index];
table.ShowTableStyleFirstColumn = true;
// Get the table style (use existing style instead of creating new one)
TableStyle style = workbook.Worksheets.TableStyles[0];
// Modify table style elements
TableStyleElement wholeTableElement = style.TableStyleElements[TableStyleElementType.WholeTable];
Style wholeTableStyle = wholeTableElement.GetElementStyle();
wholeTableStyle.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
wholeTableStyle.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
// Apply the modified style to the table
table.TableStyleName = style.Name;
// Save the workbook
workbook.Save("TableStyleElementsDemo.xlsx");
}
}
}
```
### See Also
* class [TableStyleElementCollection](../../tablestyleelementcollection/)
* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
