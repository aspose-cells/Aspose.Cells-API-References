---
title: "类 WebWorksheets"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.WebWorksheets 类。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webworksheets/
---
## WebWorksheets class

```csharp
[Obsolete("This class is obsolete; use  GridWorksheetCollection instead")]
public class WebWorksheets : ICollection, ISerializable
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [WebWorksheets](webworksheets/)(MainWeb, GridWorksheetCollection) |  |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ActiveSheet](../../aspose.cells.gridweb.data/webworksheets/activesheet/) { get; } |  |
| [ActiveSheetIndex](../../aspose.cells.gridweb.data/webworksheets/activesheetindex/) { get; set; } |  |
| [Count](../../aspose.cells.gridweb.data/webworksheets/count/) { get; } |  |
| [DefaultFontName](../../aspose.cells.gridweb.data/webworksheets/defaultfontname/) { get; set; } |  |
| [DefaultFontSize](../../aspose.cells.gridweb.data/webworksheets/defaultfontsize/) { get; set; } |  |
| [IsFixedSize](../../aspose.cells.gridweb.data/webworksheets/isfixedsize/) { get; } | 获取一个值，指示集合是否具有固定大小。 |
| [IsReadOnly](../../aspose.cells.gridweb.data/webworksheets/isreadonly/) { get; } | 获取一个值，指示 IList 是否只读。 |
| [IsSynchronized](../../aspose.cells.gridweb.data/webworksheets/issynchronized/) { get; } | 获取一个值，指示对 ICollection 的访问是否同步（线程安全）。 |
| [Item](../../aspose.cells.gridweb.data/webworksheets/item/) { get; } | 获取指定索引处的 Worksheet 元素。（2 个索引器） |
| [PivotCaches](../../aspose.cells.gridweb.data/webworksheets/pivotcaches/) { get; } | 获取 PivotCache 集合对象 |
| [PivotTables](../../aspose.cells.gridweb.data/webworksheets/pivottables/) { get; } | 获取 pivotTable 集合对象。 |
| [SyncRoot](../../aspose.cells.gridweb.data/webworksheets/syncroot/) { get; } | 获取一个可用于同步访问 ICollection 的对象。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add)() | 向集合中添加工作表。 |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_1)(object) | 添加工作表对象。 |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_2)(string) | 向集合中添加工作表。 |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_1)(int) | 向集合中添加工作表并从已有工作表复制数据。 |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_2)(string) | 向集合中添加工作表并从已有工作表复制数据。 |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy)(WebWorksheet) | 向集合中添加工作表并从已有工作表复制数据。 |
| [Clear](../../aspose.cells.gridweb.data/webworksheets/clear/)() | 清除所有工作表。 |
| [Contains](../../aspose.cells.gridweb.data/webworksheets/contains/)(object) | 指示集合是否包含该工作表。 |
| [CopyTo](../../aspose.cells.gridweb.data/webworksheets/copyto/)(Array, int) | 将内容复制到数组中。 |
| [GetEnumerator](../../aspose.cells.gridweb.data/webworksheets/getenumerator/)() |  |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview)(DataView, TableItemStyle, TableItemStyle) | 从 DataView 导入。自动使用 DataView 的表名创建工作表。 |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview_1)(DataView, TableItemStyle, TableItemStyle, string, int, int) | 从 DataView 导入到指定的工作表和位置。 |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile)(Stream) | 从 Excel 文件流导入，包括磁盘文件流或内存流。 |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile_1)(string) | 从 Excel 文件导入。 |
| [IndexOf](../../aspose.cells.gridweb.data/webworksheets/indexof/)(object) | 获取工作表的索引。 |
| [Insert](../../aspose.cells.gridweb.data/webworksheets/insert/)(int, string) | 在索引位置插入工作表。 |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile)(Stream) | 从 CSV 文件流加载数据。 |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile_1)(string) | 从 CSV 文件加载数据。 |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile)(Stream) | 从 HTML 文件流加载数据。 |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile_1)(string) | 从 HTML 文件加载数据。 |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | 从 SpreadSheetML 文件流加载数据。 |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | 从 SpreadSheetML 文件加载数据。 |
| [Remove](../../aspose.cells.gridweb.data/webworksheets/remove/)(object) | 删除工作表。 |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat)(int) | 删除索引处的工作表。 |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat_1)(string) | 删除指定名称的元素。 |
| [RunAllFormulas](../../aspose.cells.gridweb.data/webworksheets/runallformulas/)() | 运行所有单元格的公式。 |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile)(Stream) | 将数据保存到 CSV 文件流。 |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile_1)(string) | 将数据保存到 CSV 文件。 |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile)(Stream) | 将数据保存到 HTML 文件流。 |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile_1)(string) | 将数据保存到 HTML 文件。 |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | 将数据保存到 SpreadSheetML 文件流。 |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | 将数据保存到 SpreadSheetML 文件。 |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile)(Stream) | 将工作表保存到 Excel 文件流，包括磁盘 IO 流或内存流。 |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_2)(string) | 将工作表保存为 Excel 文件，使用 Excel 2003 格式。 |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | 将工作表保存到 Excel 文件。 |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_3)(string, GridSaveFormat) | 将工作表保存到 Excel 文件。 |

### 备注

注意：此类已过时。请改用 GridWorksheetCollection。此类将在自 2014 年 8 月起 6 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 另请参见

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


