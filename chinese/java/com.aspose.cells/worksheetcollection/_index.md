---
title: "WorksheetCollection"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.cells/worksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```

封装一个 [Worksheet](../../com.aspose.cells/worksheet) 对象的集合。

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
 
         //Change the name of a worksheet
         sheets.get(0).setName("First Sheet");
 
         //Set the active sheet to the second worksheet
         sheets.setActiveSheetIndex(1);
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [add()](#add--) | 向集合中添加工作表。 |
| [add(int type)](#add-int-) | 向集合中添加工作表。 |
| [add(Object o)](#add-java.lang.Object-) | 向 CollectionBase 实例添加一个项。 |
| [add(String sheetName)](#add-java.lang.String-) | 向集合中添加工作表。 |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | 复制一组工作表。 |
| [addCopy(int sheetIndex)](#addCopy-int-) | 向集合中添加工作表并从已有工作表复制数据。 |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | 向集合中添加工作表并从已有工作表复制数据。 |
| [clear()](#clear--) | 清除所有工作表。 |
| [clearPivottables()](#clearPivottables--) | 从电子表格中清除透视表。 |
| [contains(Object o)](#contains-java.lang.Object-) | 返回实例是否包含此对象 |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | 从范围地址创建一个 [Range](../../com.aspose.cells/range) 对象。 |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | 从范围地址创建一个 [Range](../../com.aspose.cells/range) 对象。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | 获取指定索引处的 [Worksheet](../../com.aspose.cells/worksheet) 元素。 |
| [get(String sheetName)](#get-java.lang.String-) | 获取具有指定名称的 [Worksheet](../../com.aspose.cells/worksheet) 元素。 |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | 表示打开电子表格时活动工作表的索引。 |
| [getActiveSheetName()](#getActiveSheetName--) | 表示在打开电子表格时活动工作表的名称。 |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | 返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有内置文档属性。 |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | 获取 CollectionBase 实例中包含的元素数量。 |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | 返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有自定义文档属性。 |
| [getDxfs()](#getDxfs--) | 获取主差异格式化记录。 |
| [getExternalLinks()](#getExternalLinks--) | 表示工作簿中的外部链接。 |
| [getNamedRanges()](#getNamedRanges--) | 获取电子表格中所有预定义的命名范围。 |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | 获取电子表格中所有预定义的命名范围。 |
| [getNames()](#getNames--) | 获取电子表格中所有 Name 对象的集合。 |
| [getOleSize()](#getOleSize--) | 获取当 Workbook 文件用作 Ole 对象时的显示大小。 |
| [getPivotCaches()](#getPivotCaches--) | 获取所有 [PivotCache](../../com.aspose.cells/pivotcache)。 |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | 通过预定义名称获取 Range 对象。 |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | 通过预定义名称或表名获取 [Range](../../com.aspose.cells/range) |
| [getRevisionLogs()](#getRevisionLogs--) | 表示修订日志。 |
| [getSensitivityLabels()](#getSensitivityLabels--) | 表示所有敏感标签。 |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | 通过代码名称获取工作表。 |
| [getTableStyles()](#getTableStyles--) | 获取 [getTableStyles()](../../com.aspose.cells/worksheetcollection\\#getTableStyles--) 对象。 |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | 获取线程评论作者的列表。 |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | 获取任务窗格的列表。 |
| [getWebExtensions()](#getWebExtensions--) | 获取任务窗格的列表。 |
| [getXmlMaps()](#getXmlMaps--) | 获取工作簿中的 XML 映射。 |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | 确定 CollectionBase 实例中特定项的索引。 |
| [insert(int index, int sheetType)](#insert-int-int-) | 插入工作表。 |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | 插入工作表。 |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | 指示在 MS Excel 中打开文件时是否刷新所有连接。 |
| [iterator()](#iterator--) | 返回遍历 CollectionBase 实例的枚举器。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | 使用数据透视源刷新所有数据透视表和图表。 |
| [refreshPivotTables()](#refreshPivotTables--) | 刷新 Excel 文件中的所有 PivotTable。 |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | 刷新 Excel 文件中的所有 PivotTable。 |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | 向工作簿添加加载项功能 |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | 向工作簿添加加载项功能 |
| [removeAt(int index)](#removeAt-int-) | 删除指定索引处的元素。 |
| [removeAt(String name)](#removeAt-java.lang.String-) | 删除指定名称的元素。 |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | 表示打开电子表格时活动工作表的索引。 |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | 表示在打开电子表格时活动工作表的名称。 |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | 设置当 Workbook 文件用作 Ole 对象时的显示大小。 |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | 设置当 Workbook 文件用作 Ole 对象时的显示大小。 |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | 指示在 MS Excel 中打开文件时是否刷新所有连接。 |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | 设置工作簿中的 XML 映射。 |
| [sortNames()](#sortNames--) | 对已定义的名称进行排序. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | 交换这两个工作表. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


向集合中添加工作表。

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) 对象索引.
### add(int type) {#add-int-}
```
public int add(int type)
```


向集合中添加工作表。

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add(SheetType.CHART);
         	Cells cells = workbook.getWorksheets().get(0).getCells();
         	cells.get("c2").putValue(5000);
         	cells.get("c3").putValue(3000);
         	cells.get("c4").putValue(4000);
         	cells.get("c5").putValue(5000);
         	cells.get("c6").putValue(6000);
         	ChartCollection charts = workbook.getWorksheets().get(1).getCharts();
         	int chartIndex = charts.add(ChartType.COLUMN, 10,10,20,20);
         	Chart chart = charts.get(chartIndex);
         	chart.getNSeries().add("Sheet1!C2:C6", true);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype)。工作表类型. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) 对象索引.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


向 CollectionBase 实例添加一个项。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 要添加到 CollectionBase 实例的对象。 |

**Returns:**
int - 新元素插入的位置。
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```


向集合中添加工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 工作表名称 |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Worksheet](../../com.aspose.cells/worksheet) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```


复制一组工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | 源工作表. |
| destSheetNames | java.lang.String[] | 已复制工作表的名称. |

### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


向集合中添加工作表并从已有工作表复制数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | int | 源工作表的索引. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) 对象索引.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


向集合中添加工作表并从已有工作表复制数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 源工作表的名称. |

**Returns:**
int - [Worksheet](../../com.aspose.cells/worksheet) 对象索引.
### clear() {#clear--}
```
public void clear()
```


清除所有工作表。

**Remarks**

工作簿必须包含一个工作表.

### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```


从电子表格中清除透视表。

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


返回实例是否包含此对象

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 测试对象 |

**Returns:**
boolean - 实例是否包含此对象
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```


从范围地址创建一个 [Range](../../com.aspose.cells/range) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 地址 | java.lang.String | 范围的地址. |
| sheetIndex | int | 工作表索引。 |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```


从范围地址创建一个 [Range](../../com.aspose.cells/range) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 地址 | java.lang.String | 范围的地址. |
| sheetIndex | int | 工作表索引。 |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```


获取指定索引处的 [Worksheet](../../com.aspose.cells/worksheet) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 元素的零基索引。 |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```


获取具有指定名称的 [Worksheet](../../com.aspose.cells/worksheet) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetName | java.lang.String | 工作表名称 |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


表示打开电子表格时活动工作表的索引。

**Remarks**

工作表索引从零开始.

**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```


表示在打开电子表格时活动工作表的名称。

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有内置文档属性。

**Remarks**

不能向内置文档属性列表添加新属性。只能获取内置属性并更改其值。以下是内置属性名称列表:

标题

主题

作者

关键字

注释

模板

最后作者

修订号

应用程序名称

最后打印日期

创建日期

最后保存时间

总编辑时间

页数

单词数

字符数

安全性

类别

格式

管理员

公司

字节数

行数

段落数

幻灯片数

备注数

隐藏幻灯片数

多媒体剪辑数

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getWorksheets().getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


获取 CollectionBase 实例中包含的元素数量。

**Returns:**
int - CollectionBase 实例中包含的元素数量。
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


返回一个 [DocumentProperty](../../com.aspose.cells/documentproperty) 集合，表示电子表格的所有自定义文档属性。

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getDxfs() {#getDxfs--}
```
public DxfCollection getDxfs()
```


获取主差异格式化记录。

**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```


表示工作簿中的外部链接。

**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```


获取电子表格中所有预定义的命名范围。

**Returns:**
com.aspose.cells.Range[] - Range 对象数组。如果定义的 Name 的引用是外部的或具有多个范围，则不会为此 Name 返回 Range 对象。

如果命名范围不存在，则返回 null。
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```


获取电子表格中所有预定义的命名范围。

**Returns:**
com.aspose.cells.Range[] - Range 对象数组。

如果命名范围不存在，则返回 null。
### getNames() {#getNames--}
```
public NameCollection getNames()
```


获取电子表格中所有 Name 对象的集合。

**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```


获取当 Workbook 文件用作 Ole 对象时的显示大小。

**Remarks**

Null 表示没有 ole 大小设置。

**Returns:**
java.lang.Object
### getPivotCaches() {#getPivotCaches--}
```
public PivotCacheCollection getPivotCaches()
```


获取所有 [PivotCache](../../com.aspose.cells/pivotcache)。

**Returns:**
[PivotCacheCollection](../../com.aspose.cells/pivotcachecollection)
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```


通过预定义名称获取 Range 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rangeName | java.lang.String | 范围的名称。 |

**Returns:**
[Range](../../com.aspose.cells/range) - Range object.

如果命名范围不存在，则返回 null。
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```


通过预定义名称或表名获取 [Range](../../com.aspose.cells/range)

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rangeName | java.lang.String | 范围的名称或表的名称。 |
| currentSheetIndex | int | 工作表索引。-1 表示全局。 |
| includeTable | boolean | 指示是否检查所有表格。 |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```


表示修订日志。

**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```


表示所有敏感标签。

**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```


通过代码名称获取工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| codeName | java.lang.String | 工作表代码名称。 |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```


获取 [getTableStyles()](../../com.aspose.cells/worksheetcollection\\#getTableStyles--) 对象。

**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```


获取线程评论作者的列表。

**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```


获取任务窗格的列表。

**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```


获取任务窗格的列表。

**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```


获取工作簿中的 XML 映射。

**Returns:**
[XmlMapCollection](../../com.aspose.cells/xmlmapcollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


确定 CollectionBase 实例中特定项的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| o | java.lang.Object | 确定 CollectionBase 实例中特定项的索引。 |

**Returns:**
int - 如果在列表中找到该值则返回其索引；否则返回 -1。
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```


插入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 工作表索引 |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). 工作表类型。 |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```


插入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 工作表索引 |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). 工作表类型。 |
| sheetName | java.lang.String | 工作表名称。 |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```


指示在 MS Excel 中打开文件时是否刷新所有连接。

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


返回遍历 CollectionBase 实例的枚举器。

**Returns:**
java.util.Iterator - 用于遍历 CollectionBase 实例的迭代器。
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


使用数据透视源刷新所有数据透视表和图表。

**Remarks**

注意：此成员现已过时。请改用 Workbook.RefreshAll() 方法。此方法将在自 2026 年 4 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


刷新 Excel 文件中的所有 PivotTable。

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


刷新 Excel 文件中的所有 PivotTable。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | 用于刷新数据透视表数据源的选项。 |

**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```


向工作簿添加加载项功能

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| id | int | 包含 addin 函数的数据的 ID，可通过对同一 addin 文件的第一次调用 [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) 获得。 |
| functionName | java.lang.String | addin 函数名称 |

**Returns:**
java.lang.String - 包含 addin 函数的 addin 文件的 URL
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```


向工作簿添加加载项功能

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| addInFile | java.lang.String | 包含 addin 函数的文件 |
| functionName | java.lang.String | addin 函数名称 |
| lib | boolean | 给定的 addin 文件是否位于 Workbook Add-In 库的目录或子目录中。当给定的 addInFile 为相对路径时，此标志生效并产生差异：true 表示路径相对于 Add‑In 库，false 表示路径相对于此 Workbook。 |

**Returns:**
int - 包含给定 addin 函数的数据的 ID
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


删除指定索引处的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 要删除的元素的索引值。 |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


删除指定名称的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String | 要删除的元素的名称。 |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


表示打开电子表格时活动工作表的索引。

**Remarks**

工作表索引从零开始.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```


表示在打开电子表格时活动工作表的名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```


设置当 Workbook 文件用作 Ole 对象时的显示大小。

**Remarks**

此方法通常用于调整 ppt 文件或 doc 文件的显示尺寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| endRow | int | 结束行索引。 |
| startColumn | int | 起始列索引。 |
| endColumn | int | 结束列索引。 |

### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```


设置当 Workbook 文件用作 Ole 对象时的显示大小。

**Remarks**

Null 表示没有 ole 大小设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.Object |  |

### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```


指示在 MS Excel 中打开文件时是否刷新所有连接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```


设置工作簿中的 XML 映射。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |

### sortNames() {#sortNames--}
```
public void sortNames()
```


对已定义的名称进行排序.

**Remarks**

如果在 Excel 文件中创建了大量命名范围，请在创建完所有命名范围并在保存之前调用此方法。

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


交换这两个工作表.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex1 | int | 第一个工作表。 |
| sheetIndex2 | int | 第二个工作表。 |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

