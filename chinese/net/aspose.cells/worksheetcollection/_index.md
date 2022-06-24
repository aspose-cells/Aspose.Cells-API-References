---
title: WorksheetCollection
second_title: Aspose.Cells for .NET API 参考
description: 封装Worksheet./worksheet对象的集合
type: docs
weight: 6520
url: /zh/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

封装[`Worksheet`](../worksheet)对象的集合。

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | 表示打开电子表格时活动工作表的索引。 |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | 表示打开电子表格时活动工作表的名称。 |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | 返回代表电子表格所有内置文档属性的[`DocumentProperty`](../../aspose.cells.properties/documentproperty)集合。 |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | 返回代表电子表格所有自定义文档属性的[`DocumentProperty`](../../aspose.cells.properties/documentproperty)集合。 |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | 获取主差分格式记录。 |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | 表示工作簿中的外部链接。 |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | 指示是否在 MS Excel 中打开文件时刷新所有连接。 |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | 获取指定索引处的[`Worksheet`](../worksheet)元素。 (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | 获取电子表格中所有 Name 对象的集合。 |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | 获取和设置工作簿文件用作 Ole 对象时的显示大小。 |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | 表示修订日志。 |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | 获取[`TableStyles`](./tablestyles)对象。 |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | 获取线程评论作者列表。 |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | 获取任务窗格列表。 |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | 获取任务窗格列表。 |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | 获取和设置工作簿中的 XML 映射。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | 将工作表添加到集合中。 |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | 将工作表添加到集合中。 |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | 将工作表添加到集合中。 |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | 将工作表添加到集合并从现有工作表复制数据。 |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | 将工作表添加到集合并从现有工作表复制数据。 |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | 清除所有工作表。 (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | 从电子表格中清除数据透视表。 |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | 从范围的地址创建[`Range`](../range)对象。 |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | 从范围的地址创建[`Range`](../range)对象。 |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | 获取电子表格中所有预定义的命名范围。 |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | 获取电子表格中所有预定义的命名范围。 |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | 通过预定义的名称获取 Range 对象。 |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | 通过预定义名称或表名获取[`Range`](../range) |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | 通过代号获取工作表。 |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | 插入工作表。 |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | 插入工作表。 |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | 刷新 WorksheetCollection 中的所有数据透视表。 |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | 将插件函数添加到工作簿 |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | 将插件函数添加到工作簿 |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | 删除指定索引处的元素。 (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | 移除指定名称的元素。 |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | 设置工作簿文件用作 Ole 对象时的显示大小。 |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | 对定义的名称进行排序。 |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | 交换两张纸。 |

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

 //添加工作表
sheets.Add();

 //更改工作表的名称
sheets[0].Name = "First Sheet";

 //将活动工作表设置为第二个工作表
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'添加工作表
sheets.Add()

'更改工作表的名称
sheets(0).Name = "First Sheet"

'将活动工作表设置为第二个工作表
sheets.ActiveSheetIndex = 1
```

### 也可以看看

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
