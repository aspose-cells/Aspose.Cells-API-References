##TableStyleCollection.AddTableStyle
TableStyleCollection method. Adds a custom table style
## TableStyleCollection.AddTableStyle method
Adds a custom table style.
```csharp
public int AddTableStyle(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The table style name. |
### Return Value
The index of the table style.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TableStyleCollectionMethodAddTableStyleWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
for (int i = 0; i < 5; i++)
{
worksheet.Cells[0, i].PutValue("Header " + (i + 1));
for (int row = 1; row < 6; row++)
{
worksheet.Cells[row, i].PutValue(row * (i + 1));
}
}
// Create a custom table style
string styleName = "MyCustomStyle";
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
int styleIndex = tableStyles.AddTableStyle(styleName);
TableStyle tableStyle = tableStyles[styleIndex];
// Style the header row
Style headerStyle = workbook.CreateStyle();
headerStyle.Font.IsBold = true;
headerStyle.ForegroundColor = System.Drawing.Color.LightBlue;
headerStyle.Pattern = BackgroundType.Solid;
tableStyle.TableStyleElements.Add(TableStyleElementType.HeaderRow);
TableStyleElement headerElement = tableStyle.TableStyleElements[TableStyleElementType.HeaderRow];
headerElement.SetElementStyle(headerStyle);
// Style the first column
Style firstColStyle = workbook.CreateStyle();
firstColStyle.Font.Color = System.Drawing.Color.Red;
tableStyle.TableStyleElements.Add(TableStyleElementType.FirstColumn);
TableStyleElement firstColElement = tableStyle.TableStyleElements[TableStyleElementType.FirstColumn];
firstColElement.SetElementStyle(firstColStyle);
// Create a table with the custom style
int tableIndex = worksheet.ListObjects.Add(0, 0, 5, 4, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.TableStyleName = styleName;
table.ShowTableStyleFirstColumn = true;
workbook.Save("CustomTableStyleDemo.xlsx");
}
}
}
```
### See Also
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
