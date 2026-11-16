---
title: "JsonSaveOptions 类"
linktitle: "JsonSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "JsonSaveOptions 类。封装在 Go 中表示 jsonsaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

表示将工作簿保存为 JSON 文件的选项。

```go

type JsonSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewJsonSaveOptions](./newjsonsaveoptions/) | 创建用于保存 json 文件的选项。 |
| [NewJsonSaveOptions_SaveOptions](./newjsonsaveoptions_saveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetExportStylePool](./getexportstylepool/) | 指示是否将样式整体导出或分别导出到每个单元格。 |
| [SetExportStylePool](./setexportstylepool/) | 指示是否将样式整体导出或分别导出到每个单元格。 |
| [GetExportHyperlinkType](./getexporthyperlinktype/) | 表示导出超链接到 json 的类型。 |
| [SetExportHyperlinkType](./setexporthyperlinktype/) | 表示导出超链接到 json 的类型。 |
| [GetSkipEmptyRows](./getskipemptyrows/) | 指示是否跳过空行。 |
| [SetSkipEmptyRows](./setskipemptyrows/) | 指示是否跳过空行。 |
| [GetSheetIndexes](./getsheetindexes/) | 表示导出工作表的索引。 |
| [SetSheetIndexes](./setsheetindexes/) | 表示导出工作表的索引。 |
| [GetSchemas](./getschemas/) | 每个工作表的原始 json 架构。 |
| [SetSchemas](./setschemas/) | 每个工作表的原始 json 架构。 |
| [GetExportArea](./getexportarea/) | 获取或设置导出范围。 |
| [SetExportArea](./setexportarea/) | 获取或设置导出范围。 |
| [GetHasHeaderRow](./gethasheaderrow/) | 指示范围是否包含标题行。 |
| [SetHasHeaderRow](./sethasheaderrow/) | 指示范围是否包含标题行。 |
| [GetExportAsString](./getexportasstring/) | 将单元格的字符串值导出为 json。 |
| [SetExportAsString](./setexportasstring/) | 将单元格的字符串值导出为 json。 |
| [GetIndent](./getindent/) | 指示缩进。 |
| [SetIndent](./setindent/) | 指示缩进。 |
| [GetExportNestedStructure](./getexportnestedstructure/) | 导出为父子层次结构的 Json 结构。 |
| [SetExportNestedStructure](./setexportnestedstructure/) | 导出为父子层次结构的 Json 结构。 |
| [GetExportEmptyCells](./getexportemptycells/) | 指示是否将空单元格导出为 null。 |
| [SetExportEmptyCells](./setexportemptycells/) | 指示是否将空单元格导出为 null。 |
| [GetAlwaysExportAsJsonObject](./getalwaysexportasjsonobject/) | 指示是否始终将 excel 导出为 json 对象，即使文件中只有一个工作表。 |
| [SetAlwaysExportAsJsonObject](./setalwaysexportasjsonobject/) | 指示是否始终将 excel 导出为 json 对象，即使文件中只有一个工作表。 |
| [GetToExcelStruct](./gettoexcelstruct/) | 指示是否将 Excel 文件转换为 json 结构体。 |
| [SetToExcelStruct](./settoexcelstruct/) | 指示是否将 Excel 文件转换为 json 结构体。 |
| [GetSaveFormat](./getsaveformat/) | 获取保存文件的格式。 |
| [GetClearData](./getcleardata/) | 在保存文件后使工作簿为空。 |
| [SetClearData](./setcleardata/) | 在保存文件后使工作簿为空。 |
| [GetCachedFileFolder](./getcachedfilefolder/) | 用于临时文件的文件夹，可用作数据缓存。 |
| [SetCachedFileFolder](./setcachedfilefolder/) | 用于临时文件的文件夹，可用作数据缓存。 |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | 指示是否在保存文件前验证合并单元格。 |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | 指示是否在保存文件前验证合并单元格。 |
| [GetMergeAreas](./getmergeareas/) | 指示是否在保存文件前合并条件格式和验证的区域。 |
| [SetMergeAreas](./setmergeareas/) | 指示是否在保存文件前合并条件格式和验证的区域。 |
| [GetCreateDirectory](./getcreatedirectory/) | 如果为 true 且目录不存在，目录将在保存文件前自动创建。 |
| [SetCreateDirectory](./setcreatedirectory/) | 如果为 true 且目录不存在，目录将在保存文件前自动创建。 |
| [GetSortNames](./getsortnames/) | 指示是否在保存文件前对已定义名称进行排序。 |
| [SetSortNames](./setsortnames/) | 指示是否在保存文件前对已定义名称进行排序。 |
| [GetSortExternalNames](./getsortexternalnames/) | 指示是否在保存文件前对外部已定义名称进行排序。 |
| [SetSortExternalNames](./setsortexternalnames/) | 指示是否在保存文件前对外部已定义名称进行排序。 |
| [GetRefreshChartCache](./getrefreshchartcache/) | 指示是否缓存图表的最新数据。 |
| [SetRefreshChartCache](./setrefreshchartcache/) | 指示是否缓存图表的最新数据。 |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | 是否在用户修改与单元格相关的对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当输入的值超过 32K 时，将被截断。 |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | 是否在用户修改与单元格相关的对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当输入的值超过 32K 时，将被截断。 |
| [GetUpdateSmartArt](./getupdatesmartart/) | 指示是否更新 Smart Art 设置。默认值为 false。 |
| [SetUpdateSmartArt](./setupdatesmartart/) | 指示是否更新 Smart Art 设置。默认值为 false。 |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。 |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。 |
