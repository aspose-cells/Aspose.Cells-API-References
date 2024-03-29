---
title: ListObject
second_title: Aspose.Cells for .NET API 参考
description: 表示工作表上的列表对象 ListObject 对象是 ListObjects 集合的成员 ListObjects 集合包含工作表上的所有列表对象
type: docs
weight: 5820
url: /zh/net/aspose.cells.tables/listobject/
---
## ListObject class

表示工作表上的列表对象。 ListObject 对象是 ListObjects 集合的成员。 ListObjects 集合包含工作表上的所有列表对象。

```csharp
public class ListObject
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AlternativeDescription](../../aspose.cells.tables/listobject/alternativedescription) { get; set; } | 获取和设置替代描述。 |
| [AlternativeText](../../aspose.cells.tables/listobject/alternativetext) { get; set; } | 获取和设置替代文本。 |
| [AutoFilter](../../aspose.cells.tables/listobject/autofilter) { get; } | 获取自动过滤器。 |
| [Comment](../../aspose.cells.tables/listobject/comment) { get; set; } | 获取和设置表格的注释。 |
| [DataRange](../../aspose.cells.tables/listobject/datarange) { get; } | 获取ListObject的数据范围。 |
| [DataSourceType](../../aspose.cells.tables/listobject/datasourcetype) { get; } | 获取表的数据源类型。 |
| [DisplayName](../../aspose.cells.tables/listobject/displayname) { get; set; } | 获取和设置显示名称。 |
| [EndColumn](../../aspose.cells.tables/listobject/endcolumn) { get; } | 获取范围的结束列。 |
| [EndRow](../../aspose.cells.tables/listobject/endrow) { get; } | 获取范围的结束行。 |
| [ListColumns](../../aspose.cells.tables/listobject/listcolumns) { get; } | 获取 ListObject 的 ListColumns。 |
| [QueryTable](../../aspose.cells.tables/listobject/querytable) { get; } | 获取链接的QueryTable。 |
| [ShowHeaderRow](../../aspose.cells.tables/listobject/showheaderrow) { get; set; } | 获取并设置此 ListObject 是否显示标题行。 |
| [ShowTableStyleColumnStripes](../../aspose.cells.tables/listobject/showtablestylecolumnstripes) { get; set; } | 指示是否应用列带格式。 |
| [ShowTableStyleFirstColumn](../../aspose.cells.tables/listobject/showtablestylefirstcolumn) { get; set; } | 指示表中的第一列是否应应用样式。 |
| [ShowTableStyleLastColumn](../../aspose.cells.tables/listobject/showtablestylelastcolumn) { get; set; } | 指示表中的最后一列是否应应用样式。 |
| [ShowTableStyleRowStripes](../../aspose.cells.tables/listobject/showtablestylerowstripes) { get; set; } | 指示是否应用行条纹格式。 |
| [ShowTotals](../../aspose.cells.tables/listobject/showtotals) { get; set; } | 获取并设置此 ListObject 是否显示总行。 |
| [StartColumn](../../aspose.cells.tables/listobject/startcolumn) { get; } | 获取范围的起始列。 |
| [StartRow](../../aspose.cells.tables/listobject/startrow) { get; } | 获取范围的起始行。 |
| [TableStyleName](../../aspose.cells.tables/listobject/tablestylename) { get; set; } | 获取和设置表格样式名称。 |
| [TableStyleType](../../aspose.cells.tables/listobject/tablestyletype) { get; set; } | 获取和内置表格样式。 |
| [XmlMap](../../aspose.cells.tables/listobject/xmlmap) { get; } | 得到一个[`XmlMap`](./xmlmap)用于此列表。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [ApplyStyleToRange](../../aspose.cells.tables/listobject/applystyletorange)() | 将表格样式应用于范围。 |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange)() | 将表格转换为范围。 |
| [ConvertToRange](../../aspose.cells.tables/listobject/converttorange#converttorange_1)(TableToRangeOptions) | 将表格转换为范围。 |
| [Filter](../../aspose.cells.tables/listobject/filter)() | 过滤表。 |
| [PutCellValue](../../aspose.cells.tables/listobject/putcellvalue)(int, int, object) | 将值放入单元格。 |
| [Resize](../../aspose.cells.tables/listobject/resize)(int, int, int, int, bool) | 调整列表对象的范围。 |
| [UpdateColumnName](../../aspose.cells.tables/listobject/updatecolumnname)() | 更新工作表中所有列表列的名称。 |

### 例子

```csharp

[C#]


Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
for (int i = 0; i  <5; i++)
{
cells[0,i].PutValue(CellsHelper.ColumnIndexToName(i));
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
table.ShowTotals = true;
table.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
workbook.Save(@"Book1.xlsx");


[Visual Basic]

Dim workbook As Workbook = New Workbook()
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
table.ShowTotals = True
table.ListColumns(4).TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum
workbook.Save("Book1.xlsx")
```

### 也可以看看

* 命名空间 [Aspose.Cells.Tables](../../aspose.cells.tables)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
