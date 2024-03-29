---
title: TxtSaveOptions
second_title: Aspose.Cells for .NET API 参考
description: 表示 csv/制表符分隔/其他文本格式的保存选项
type: docs
weight: 6130
url: /zh/net/aspose.cells/txtsaveoptions/
---
## TxtSaveOptions class

表示 csv/制表符分隔/其他文本格式的保存选项。

```csharp
public class TxtSaveOptions : SaveOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [TxtSaveOptions](txtsaveoptions#constructor)() | 创建文本文件保存选项。 |
| [TxtSaveOptions](txtsaveoptions#constructor_1)(SaveFormat) | 创建文本文件保存选项。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | 缓存的文件夹是用来存放一些大数据的。 |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | 保存文件后使工作簿为空。 |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | 如果为true且目录不存在，会在保存文件前自动创建目录。 |
| [Encoding](../../aspose.cells/txtsaveoptions/encoding) { get; set; } | 获取并设置默认编码。 |
| [ExportAllSheets](../../aspose.cells/txtsaveoptions/exportallsheets) { get; set; } | 表示是否将所有工作表导出到文本文件。 如果为false，则只导出活动工作表，就像MS Excel一样。 |
| [ExportArea](../../aspose.cells/txtsaveoptions/exportarea) { get; set; } | 要导出的单元格范围。 |
| [ExportQuotePrefix](../../aspose.cells/txtsaveoptions/exportquoteprefix) { get; set; } | 指示单引号是否应作为一个单元格 值的一部分导出[`QuotePrefix`](../style/quoteprefix)是真的。默认为假。 |
| [FormatStrategy](../../aspose.cells/txtsaveoptions/formatstrategy) { get; set; } | 获取和设置单元格值导出为字符串时的格式策略。 |
| [KeepSeparatorsForBlankRow](../../aspose.cells/txtsaveoptions/keepseparatorsforblankrow) { get; set; } | 指示是否应为空白行输出分隔符。 默认值为 false，因此默认情况下空白行的内容将为空。 |
| [LightCellsDataProvider](../../aspose.cells/txtsaveoptions/lightcellsdataprovider) { get; set; } | 提供单元格数据以在轻量模式下保存工作簿的数据提供程序。 |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | 表示是否在保存文件之前合并条件格式和验证区域。 |
| [QuoteType](../../aspose.cells/txtsaveoptions/quotetype) { get; set; } | 获取或设置如何在导出的文本文件中引用值。 |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | 表示是否刷新图表缓存数据 |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | 获取保存文件格式。 |
| [Separator](../../aspose.cells/txtsaveoptions/separator) { get; set; } | 获取和设置文本文件的字符分隔符。 |
| [SeparatorString](../../aspose.cells/txtsaveoptions/separatorstring) { get; set; } | 获取并设置一个字符串值作为分隔符。 |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | 表示是否在保存文件之前对外部定义的名称进行排序。 |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | 表示是否在保存文件之前对定义的名称进行排序。 |
| [TrimLeadingBlankRowAndColumn](../../aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn) { get; set; } | 指示是否应该像 ms excel 那样修剪前导空白行和列。 默认为 true。 |
| [TrimTailingBlankCells](../../aspose.cells/txtsaveoptions/trimtailingblankcells) { get; set; } | 指示是否应修剪一行中的拖尾空白单元格。默认为假。 |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | 表示是否更新智能艺术设置。 默认值为false。 |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | 表示是否在保存文件之前验证合并的单元格。 |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | 获取或设置警告回调。 |

### 也可以看看

* class [SaveOptions](../saveoptions)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
