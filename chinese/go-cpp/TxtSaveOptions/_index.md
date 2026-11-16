---
title: "TxtSaveOptions 类"
linktitle: "TxtSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "TxtSaveOptions 类。封装了在 Go 中表示 txtsaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/txtsaveoptions/
---

## TxtSaveOptions class

表示 csv/制表符分隔/其他文本格式的保存选项。

```go

type TxtSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewTxtSaveOptions](./newtxtsaveoptions/) | 创建文本文件保存选项。 |
| [NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | 创建文本文件保存选项。 |
| [NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetSeparator](./getseparator/) | 获取并设置文本文件的字符分隔符。 |
| [SetSeparator](./setseparator/) | 获取并设置文本文件的字符分隔符。 |
| [GetSeparatorString](./getseparatorstring/) | 获取并设置字符串值作为分隔符。 |
| [SetSeparatorString](./setseparatorstring/) | 获取并设置字符串值作为分隔符。 |
| [GetEncoding](./getencoding/) | 获取并设置默认编码。 |
| [SetEncoding](./setencoding/) | 获取并设置默认编码。 |
| [GetQuoteType](./getquotetype/) | 获取或设置在导出文本文件中如何为值加引号。 |
| [SetQuoteType](./setquotetype/) | 获取或设置在导出文本文件中如何为值加引号。 |
| [GetFormatStrategy](./getformatstrategy/) | 获取并设置导出单元格值为字符串时的格式策略。 |
| [SetFormatStrategy](./setformatstrategy/) | 获取并设置导出单元格值为字符串时的格式策略。 |
| [GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | 指示是否应像 MS Excel 那样修剪前导空行和空列。默认值为 true。 |
| [SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | 指示是否应像 MS Excel 那样修剪前导空行和空列。默认值为 true。 |
| [GetTrimTailingBlankCells](./gettrimtailingblankcells/) | 指示是否应修剪一行中尾部的空单元格。默认值为 false。 |
| [SetTrimTailingBlankCells](./settrimtailingblankcells/) | 指示是否应修剪一行中尾部的空单元格。默认值为 false。 |
| [GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | 指示是否应为空行输出分隔符。默认值为 false，因此默认情况下空行的内容将为空。 |
| [SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | 指示是否应为空行输出分隔符。默认值为 false，因此默认情况下空行的内容将为空。 |
| [GetExportArea](./getexportarea/) | 要导出的单元格范围。 |
| [SetExportArea](./setexportarea/) | 要导出的单元格范围。 |
| [GetExportQuotePrefix](./getexportquoteprefix/) | 指示当 Style.QuotePrefix 为 true 时，单引号符号是否应作为单元格值的一部分导出。默认值为 false。 |
| [SetExportQuotePrefix](./setexportquoteprefix/) | 指示当 Style.QuotePrefix 为 true 时，单引号符号是否应作为单元格值的一部分导出。默认值为 false。 |
| [GetExportAllSheets](./getexportallsheets/) | 指示是否将所有工作表导出到文本文件。如果为 false，则仅导出活动工作表，类似于 MS Excel。 |
| [SetExportAllSheets](./setexportallsheets/) | 指示是否将所有工作表导出到文本文件。如果为 false，则仅导出活动工作表，类似于 MS Excel。 |
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
