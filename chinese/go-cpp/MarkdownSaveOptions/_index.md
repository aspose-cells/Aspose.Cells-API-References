---
title: "MarkdownSaveOptions 类"
linktitle: "MarkdownSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "MarkdownSaveOptions 类。封装在 Go 中表示 markdownsaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

表示 Markdown 的保存选项。

```go

type MarkdownSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewMarkdownSaveOptions](./newmarkdownsaveoptions/) | 创建用于保存 markdown 文档的选项 |
| [NewMarkdownSaveOptions_SaveOptions](./newmarkdownsaveoptions_saveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetEncoding](./getencoding/) | 获取并设置默认编码。 |
| [SetEncoding](./setencoding/) | 获取并设置默认编码。 |
| [GetFormatStrategy](./getformatstrategy/) | 获取并设置导出单元格值为字符串时的格式策略。 |
| [SetFormatStrategy](./setformatstrategy/) | 获取并设置导出单元格值为字符串时的格式策略。 |
| [GetLineSeparator](./getlineseparator/) | 获取和设置行分隔符。 |
| [SetLineSeparator](./setlineseparator/) | 获取和设置行分隔符。 |
| [GetTableHeaderType](./gettableheadertype/) | 获取和设置表格标题的方式。 |
| [SetTableHeaderType](./settableheadertype/) | 获取和设置表格标题的方式。 |
| [GetSheetSet](./getsheetset/) | 获取或设置要渲染的工作表。默认是工作簿中所有可见工作表：Aspose.Cells.Rendering.SheetSet.Active。 |
| [SetSheetSet](./setsheetset/) | 获取或设置要渲染的工作表。默认是工作簿中所有可见工作表：Aspose.Cells.Rendering.SheetSet.Active。 |
| [GetImageOptions](./getimageoptions/) | 在导出之前获取 ImageOrPrintOptions 对象。 |
| [GetExportImagesAsBase64](./getexportimagesasbase64/) | 指定是否将图像以 Base64 格式保存到 Markdown。默认值为 true。 |
| [SetExportImagesAsBase64](./setexportimagesasbase64/) | 指定是否将图像以 Base64 格式保存到 Markdown。默认值为 true。 |
| [GetCalculateFormula](./getcalculateformula/) | 指示是否在保存 markdown 文件之前计算公式。 |
| [SetCalculateFormula](./setcalculateformula/) | 指示是否在保存 markdown 文件之前计算公式。 |
| [GetExportHyperlinkAsReference](./getexporthyperlinkasreference/) | 指示是否使用引用定义而不是内联格式导出超链接。默认值为 false。 |
| [SetExportHyperlinkAsReference](./setexporthyperlinkasreference/) | 指示是否使用引用定义而不是内联格式导出超链接。默认值为 false。 |
| [GetAlignColumnPadding](./getaligncolumnpadding/) | 指示是否为生成的 Markdown 表启用列对齐。启用时，列通过使用指定字符（通常是空格 ' '）填充单元格内容来对齐。将其设置为 '\\0' 可禁用列对齐（默认）。 |
| [SetAlignColumnPadding](./setaligncolumnpadding/) | 指示是否为生成的 Markdown 表启用列对齐。启用时，列通过使用指定字符（通常是空格 ' '）填充单元格内容来对齐。将其设置为 '\\0' 可禁用列对齐（默认）。 |
| [GetSplitTablesByBlankRow](./getsplittablesbyblankrow/) | 指示在导出为 Markdown 时，工作表中的空白行是否应视为表格分隔符。默认值为 false。 |
| [SetSplitTablesByBlankRow](./setsplittablesbyblankrow/) | 指示在导出为 Markdown 时，工作表中的空白行是否应视为表格分隔符。默认值为 false。 |
| [GetOfficeMathOutputType](./getofficemathoutputtype/) | 指示 OfficeMath 对象如何导出为 Markdown，默认值为 Image。 |
| [SetOfficeMathOutputType](./setofficemathoutputtype/) | 指示 OfficeMath 对象如何导出为 Markdown，默认值为 Image。 |
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
