---
title: Class TableStyle
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Tables.TableStyle class. Represents the table style
type: docs
url: /net/aspose.cells.tables/tablestyle/
---
## TableStyle class

Represents the table style.

```csharp
public class TableStyle
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.cells.tables/tablestyle/name/) { get; } | Gets the name of table style. |
| [TableStyleElements](../../aspose.cells.tables/tablestyle/tablestyleelements/) { get; } | Gets all elements of the table style. |

### Examples

```csharp

[C#]

Workbook workbook = new Workbook();
Style firstColumnStyle = workbook.CreateStyle();
firstColumnStyle.Pattern = BackgroundType.Solid;
firstColumnStyle.BackgroundColor = System.Drawing.Color.Red;

Style lastColumnStyle = workbook.CreateStyle();
lastColumnStyle.Font.IsBold = true;
lastColumnStyle.Pattern = BackgroundType.Solid;
lastColumnStyle.BackgroundColor = System.Drawing.Color.Red;
string tableStyleName = "Custom1";
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
int index1 = tableStyles.AddTableStyle(tableStyleName);
TableStyle tableStyle = tableStyles[index1];
TableStyleElementCollection elements = tableStyle.TableStyleElements;
index1 = elements.Add(TableStyleElementType.FirstColumn);
TableStyleElement element = elements[index1];
element.SetElementStyle(firstColumnStyle);
index1 = elements.Add(TableStyleElementType.LastColumn);
element = elements[index1];
element.SetElementStyle(lastColumnStyle);
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i  <5; i++)
{
    cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
}
for (int row = 1; row  <10; row++)
{
    for (int column = 0; column  <5; column++)
    {
        cells[row, column].PutValue(row * column);
    }
 }
ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
int index = tables.Add(0, 0, 9, 4, true);
ListObject table = tables[0];
table.ShowTableStyleFirstColumn = true;
table.ShowTableStyleLastColumn = true;
table.TableStyleName = tableStyleName;
workbook.Save(@"Book1.xlsx");

[Visual Basic]

  Dim workbook As Workbook = New Workbook()
Dim firstColumnStyle As Style = workbook.CreateStyle()
firstColumnStyle.Pattern = BackgroundType.Solid
firstColumnStyle.BackgroundColor = System.Drawing.Color.Red
Dim lastColumnStyle As Style = workbook.CreateStyle()

lastColumnStyle.Font.IsBold = True
lastColumnStyle.Pattern = BackgroundType.Solid
lastColumnStyle.BackgroundColor = System.Drawing.Color.Red
Dim tableStyleName As String = "Custom1"

Dim tableStyles As TableStyleCollection = workbook.Worksheets.TableStyles
Dim index1 As Int32 = tableStyles.AddTableStyle(tableStyleName)
Dim tableStyle As TableStyle = tableStyles(index1)
Dim elements As TableStyleElementCollection = tableStyle.TableStyleElements
index1 = elements.Add(TableStyleElementType.FirstColumn)
Dim element As TableStyleElement = elements(index1)
element.SetElementStyle(firstColumnStyle)
index1 = elements.Add(TableStyleElementType.LastColumn)
element = elements(index1)
element.SetElementStyle(lastColumnStyle)
Dim cells As Cells = workbook.Worksheets(0).Cells
For i As Int32 = 0 To 4
    cells(0, i).PutValue(CellsHelper.ColumnIndexToName(i))
Next
For row As Int32 = 1 To 9
    For column As Int32 = 0 To 4
        cells(row, column).PutValue(row * column)
    Next
Next
Dim tables As ListObjectCollection = workbook.Worksheets(0).ListObjects
Dim index As Int32 = tables.Add(0, 0, 9, 4, True)
Dim table As ListObject = tables(0)
table.ShowTableStyleFirstColumn = True
table.ShowTableStyleLastColumn = True
table.TableStyleName = tableStyleName
workbook.Save("Book1.xlsx")
```

### See Also

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


