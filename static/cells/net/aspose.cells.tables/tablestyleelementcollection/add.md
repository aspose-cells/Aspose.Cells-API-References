##TableStyleElementCollection.Add
TableStyleElementCollection method. Adds an element
## TableStyleElementCollection.Add method
Adds an element.
```csharp
public int Add(TableStyleElementType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | TableStyleElementType | The type of the element |
### Return Value
Returns the index of the element in the list.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TableStyleElementCollectionMethodAddWithTableStyleElementTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Style firstColumnStyle = workbook.CreateStyle();
firstColumnStyle.Pattern = BackgroundType.Solid;
firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;
Style lastColumnStyle = workbook.CreateStyle();
lastColumnStyle.Font.IsBold = true;
lastColumnStyle.Pattern = BackgroundType.Solid;
lastColumnStyle.BackgroundColor = System.Drawing.Color.Blue;
string tableStyleName = "CustomStyle1";
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
int tableStyleIndex = tableStyles.AddTableStyle(tableStyleName);
TableStyle tableStyle = tableStyles[tableStyleIndex];
TableStyleElementCollection elements = tableStyle.TableStyleElements;
int elementIndex = elements.Add(TableStyleElementType.FirstColumn);
elements[elementIndex].SetElementStyle(firstColumnStyle);
elementIndex = elements.Add(TableStyleElementType.LastColumn);
elements[elementIndex].SetElementStyle(lastColumnStyle);
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i < 5; i++)
{
cells[0, i].PutValue($"Column {i + 1}");
}
int tableIndex = workbook.Worksheets[0].ListObjects.Add(0, 0, 1, 4, true);
ListObject table = workbook.Worksheets[0].ListObjects[tableIndex];
table.ShowTableStyleFirstColumn = true;
table.ShowTableStyleLastColumn = true;
table.TableStyleName = tableStyleName;
workbook.Save("TableStyleElementCollectionAddDemo.xlsx");
}
}
}
```
### See Also
* enum [TableStyleElementType](../../tablestyleelementtype/)
* class [TableStyleElementCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
