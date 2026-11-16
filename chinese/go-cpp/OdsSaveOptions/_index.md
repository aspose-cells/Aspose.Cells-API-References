---
title: "OdsSaveOptions 类"
linktitle: "OdsSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "OdsSaveOptions 类。封装了在 Go 中表示 odssaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/odssaveoptions/
---

## OdsSaveOptions class

表示保存 ODS 文件的选项。

```go

type OdsSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewOdsSaveOptions](./newodssaveoptions/) | 创建保存 ODS 文件的选项。 |
| [NewOdsSaveOptions_SaveFormat](./newodssaveoptions_saveformat/) | 创建保存 ODS 文件的选项。 |
| [NewOdsSaveOptions_SaveOptions](./newodssaveoptions_saveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetGeneratorType](./getgeneratortype/) | 获取并设置 ODS 文件的生成器。 |
| [SetGeneratorType](./setgeneratortype/) | 获取并设置 ODS 文件的生成器。 |
| [GetOdfStrictVersion](./getodfstrictversion/) | 获取并设置 ODF 版本。 |
| [SetOdfStrictVersion](./setodfstrictversion/) | 获取并设置 ODF 版本。 |
| [GetIgnorePivotTables](./getignorepivottables/) | 指示是否保存数据透视表。 |
| [SetIgnorePivotTables](./setignorepivottables/) | 指示是否保存数据透视表。 |
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
