##TableStyleElementCollection.Item
TableStyleElementCollection property. Gets an element of the table style by the index
## TableStyleElementCollection indexer (1 of 2)
Gets an element of the table style by the index.
```csharp
public TableStyleElement this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Return Value
Returns [`TableStyleElement`](../../tablestyleelement/) object
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TableStyleElementCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Style firstColStyle = workbook.CreateStyle();
firstColStyle.Pattern = BackgroundType.Solid;
firstColStyle.BackgroundColor = System.Drawing.Color.LightBlue;
string styleName = "CustomTableStyle";
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
int styleIndex = tableStyles.AddTableStyle(styleName);
TableStyle tableStyle = tableStyles[styleIndex];
TableStyleElementCollection elements = tableStyle.TableStyleElements;
int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
TableStyleElement element = elements[elementIndex];
element.SetElementStyle(firstColStyle);
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue("Header");
cells["A2"].PutValue("Data");
int tableIndex = workbook.Worksheets[0].ListObjects.Add(0, 0, 1, 0, true);
ListObject table = workbook.Worksheets[0].ListObjects[tableIndex];
table.ShowTableStyleFirstColumn = true;
table.TableStyleName = styleName;
workbook.Save("TableStyleElementDemo.xlsx");
}
}
}
```
### See Also
* class [TableStyleElement](../../tablestyleelement/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
## TableStyleElementCollection indexer (2 of 2)
Gets the element of the table style by the element type.
```csharp
public TableStyleElement this[TableStyleElementType type] { get; }
```
| Parameter | Description |
| --- | --- |
| type | The element type. |
### Return Value
Returns [`TableStyleElement`](../../tablestyleelement/) object
### See Also
* class [TableStyleElement](../../tablestyleelement/)
* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
