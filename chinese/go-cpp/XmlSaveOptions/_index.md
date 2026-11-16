---
title: "XmlSaveOptions 类"
linktitle: "XmlSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "XmlSaveOptions 类。封装在 Go 中表示 xmlsaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/xmlsaveoptions/
---

## XmlSaveOptions class

表示将工作簿保存为 xml 文件的选项。

```go

type XmlSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewXmlSaveOptions](./newxmlsaveoptions/) | 创建用于保存 XML 文件的选项。 |
| [NewXmlSaveOptions_SaveOptions](./newxmlsaveoptions_saveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetSheetIndexes](./getsheetindexes/) | 表示导出工作表的索引。 |
| [SetSheetIndexes](./setsheetindexes/) | 表示导出工作表的索引。 |
| [GetExportArea](./getexportarea/) | 获取或设置导出范围。 |
| [SetExportArea](./setexportarea/) | 获取或设置导出范围。 |
| [GetHasHeaderRow](./gethasheaderrow/) | 指示范围是否包含标题行。 |
| [SetHasHeaderRow](./sethasheaderrow/) | 指示范围是否包含标题行。 |
| [GetXmlMapName](./getxmlmapname/) | 指示是否在文件中导出 XML 映射。 |
| [SetXmlMapName](./setxmlmapname/) | 指示是否在文件中导出 XML 映射。 |
| [GetSheetNameAsElementName](./getsheetnameaselementname/) | 指示是否将工作表名称导出为元素的名称。 |
| [SetSheetNameAsElementName](./setsheetnameaselementname/) | 指示是否将工作表名称导出为元素的名称。 |
| [GetDataAsAttribute](./getdataasattribute/) | 指示是否将导出数据作为元素的属性。 |
| [SetDataAsAttribute](./setdataasattribute/) | 指示是否将导出数据作为元素的属性。 |
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
