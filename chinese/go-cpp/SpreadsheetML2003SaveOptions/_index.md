---
title: "SpreadsheetML2003SaveOptions 类"
linktitle: "SpreadsheetML2003SaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SpreadsheetML2003SaveOptions 类。封装在 Go 中表示 spreadsheetml2003saveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/spreadsheetml2003saveoptions/
---

## SpreadsheetML2003SaveOptions class

表示保存 Excel 2003 spreadml 文件的选项。

```go

type SpreadsheetML2003SaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewSpreadsheetML2003SaveOptions](./newspreadsheetml2003saveoptions/) | 创建用于保存 Excel 2003 spreadml 文件的选项。 |
| [NewSpreadsheetML2003SaveOptions_SaveOptions](./newspreadsheetml2003saveoptions_saveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [IsIndentedFormatting](./isindentedformatting/) | 导致子元素缩进。 |
| [SetIsIndentedFormatting](./setisindentedformatting/) | 导致子元素缩进。 |
| [GetLimitAsXls](./getlimitasxls/) | 以 xls 为限制，最大行索引为 65535，最大列索引为 255。 |
| [SetLimitAsXls](./setlimitasxls/) | 以 xls 为限制，最大行索引为 65535，最大列索引为 255。 |
| [GetExportColumnIndexOfCell](./getexportcolumnindexofcell/) | 默认值为 false，这意味着如果单元格与前一个单元格相邻，则列索引将被忽略。 |
| [SetExportColumnIndexOfCell](./setexportcolumnindexofcell/) | 默认值为 false，这意味着如果单元格与前一个单元格相邻，则列索引将被忽略。 |
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
