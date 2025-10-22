##Enum TableStyleElementType
Aspose.Cells.Tables.TableStyleElementType enum. Represents the Table or PivotTable style element type
## TableStyleElementType enumeration
Represents the Table or PivotTable style element type.
```csharp
public enum TableStyleElementType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| BlankRow | `18` | Table style element that applies to PivotTable's blank rows. |
| FirstColumn | `8` | Table style element that applies to table's first column. |
| FirstColumnStripe | `3` | Table style element that applies to table's first column stripes. |
| FirstColumnSubheading | `22` | Table style element that applies to PivotTable's first column subheading. |
| FirstHeaderCell | `11` | Table style element that applies to table's first header row cell. |
| FirstRowStripe | `5` | Table style element that applies to table's first row stripes. |
| FirstRowSubheading | `25` | Table style element that applies to PivotTable's first row subheading. |
| FirstSubtotalColumn | `15` | Table style element that applies to PivotTable's first subtotal column. |
| FirstSubtotalRow | `19` | Table style element that applies to pivot table's first subtotal row. |
| GrandTotalColumn | `28` | Table style element that applies to pivot table's grand total column. |
| GrandTotalRow | `29` | Table style element that applies to pivot table's grand total row. |
| FirstTotalCell | `13` | Table style element that applies to table's first total row cell. |
| HeaderRow | `9` | Table style element that applies to table's header row. |
| LastColumn | `7` | Table style element that applies to table's last column. |
| LastHeaderCell | `12` | Table style element that applies to table's last header row cell. |
| LastTotalCell | `14` | Table style element that applies to table's last total row cell. |
| PageFieldLabels | `1` | Table style element that applies to pivot table's page field labels. |
| PageFieldValues | `2` | Table style element that applies to pivot table's page field values. |
| SecondColumnStripe | `4` | Table style element that applies to table's second column stripes. |
| SecondColumnSubheading | `23` | Table style element that applies to pivot table's second column subheading. |
| SecondRowStripe | `6` | Table style element that applies to table's second row stripes. |
| SecondRowSubheading | `26` | Table style element that applies to pivot table's second row subheading. |
| SecondSubtotalColumn | `16` | Table style element that applies to PivotTable's second subtotal column. |
| SecondSubtotalRow | `20` | Table style element that applies to PivotTable's second subtotal row. |
| ThirdColumnSubheading | `24` | Table style element that applies to PivotTable's third column subheading. |
| ThirdRowSubheading | `27` | Table style element that applies to PivotTable's third row subheading. |
| ThirdSubtotalColumn | `17` | Table style element that applies to pivot table's third subtotal column. |
| ThirdSubtotalRow | `21` | Table style element that applies to PivotTable's third subtotal row. |
| TotalRow | `10` | Table style element that applies to table's total row. |
| WholeTable | `0` | Table style element that applies to table's entire content. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TablesClassTableStyleElementTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Style firstColumnStyle = workbook.CreateStyle();
firstColumnStyle.Pattern = BackgroundType.Solid;
firstColumnStyle.ForegroundColor = System.Drawing.Color.LightBlue;
Style lastColumnStyle = workbook.CreateStyle();
lastColumnStyle.Font.IsBold = true;
lastColumnStyle.Pattern = BackgroundType.Solid;
lastColumnStyle.ForegroundColor = System.Drawing.Color.LightGreen;
string tableStyleName = "CustomStyle1";
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
int styleIndex = tableStyles.AddTableStyle(tableStyleName);
TableStyle tableStyle = tableStyles[styleIndex];
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
for (int row = 1; row < 5; row++)
{
for (int col = 0; col < 5; col++)
{
cells[row, col].PutValue(row * col);
}
}
ListObject table = workbook.Worksheets[0].ListObjects[workbook.Worksheets[0].ListObjects.Add(0, 0, 4, 4, true)];
table.ShowTableStyleFirstColumn = true;
table.ShowTableStyleLastColumn = true;
table.TableStyleName = tableStyleName;
workbook.Save("TableStyleDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)
