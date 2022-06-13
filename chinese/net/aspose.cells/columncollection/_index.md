---
title: ColumnCollection
second_title: Aspose.Cells for .NET API 参考
description: 对象的集合代表工作表中的各个列设置 Column 对象仅表示列宽样式等设置对于整列 与相应列中是否存在非空单元格数据无关 而这个集合的Count只代表这个集合中已经实例化的count个Column对象 与有非空单元格无关数据或不在工作表中
type: docs
weight: 1070
url: /zh/net/aspose.cells/columncollection/
---
## ColumnCollection class

对象的集合，代表工作表中的各个列（设置）。 Column 对象仅表示列宽、样式等设置。对于整列， 与相应列中是否存在非空单元格（数据）无关。 而这个集合的“Count”只代表这个集合中已经实例化的count个Column对象， 与有非空单元格无关（数据）或不在工作表中。

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/columncollection/item) { get; } | 按列索引获取对象。 如果给定列索引的 Column 对象之前不存在，它将被实例化。 |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Column&gt;) |  |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex)(int) | 通过列表中的位置获取[`Column`](../column)对象。 |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### 例子

```csharp

[C#]

 //实例化一个工作簿对象
Workbook workbook = new Workbook();

//获取第一个worksheet

Worksheet worksheet = workbook.Worksheets[0];

//向 Workbook

Style style = workbook.CreateStyle();

//设置背景颜色为Blue
style.ForegroundColor = Color.Blue;

 //设置背景图案
style.Pattern = BackgroundType.Solid;

 //新样式标志
StyleFlag styleFlag = new StyleFlag();

 //设置所有样式
styleFlag.All = true;

 //改变前十列的默认宽度
for (int i = 0; i < 10; i++)
{
    worksheet.Cells.Columns[i].Width = 20;
}

 //获取非默认格式的Column
ColumnCollection columns = worksheet.Cells.Columns;

foreach (Column column in columns)
{
     //将样式应用于前十列
    column.ApplyStyle(style, styleFlag);
}

 //保存Excel文件
workbook.Save("book1.xls");

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the first worksheet
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Add new Style to Workbook
Dim style As Style = workbook.CreateStyles()

'Setting the background color to Blue
style.ForegroundColor = Color.Blue

'setting Background Pattern
style.Pattern = BackgroundType.Solid

'New Style Flag
Dim styleFlag As New StyleFlag()

'Set All Styles
styleFlag.All = True

'Change the default width of first ten columns
For i As Integer = 0 To 9
    worksheet.Cells.Columns(i).Width = 20
Next i

'Get the Column with non default formatting
Dim columns As ColumnCollection = worksheet.Cells.Columns

For Each column As Column In columns
    'Apply Style to first ten Columns
    column.ApplyStyle(style, styleFlag)
Next column

'Saving the Excel file
workbook.Save("book1.xls")

```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Column](../column)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->