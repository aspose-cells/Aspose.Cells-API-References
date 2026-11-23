---
title: "类 GridPdfSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridDesktop.Data.GridPdfSaveOptions 类。表示保存 PDF 文件的选项"
type: docs
url: /zh/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/
---
## GridPdfSaveOptions class

表示保存 pdf 文件的选项。

```csharp
public class GridPdfSaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GridPdfSaveOptions](gridpdfsaveoptions/)() | GridSaveOptions 的构造 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CachedFileFolder](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/cachedfilefolder/) { get; set; } | 缓存文件夹用于存储一些大数据。 |
| [CalculateFormula](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/calculateformula/) { get; set; } | 指示是否在保存 pdf 文件之前计算公式。 |
| [ClearData](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/cleardata/) { get; set; } | 在保存文件后使工作簿为空。 |
| [Compliance](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/compliance/) { get; set; } | 工作簿转换为 pdf 将遵循此属性中的 PdfCompliance。 |
| [CreateDirectory](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/createdirectory/) { get; set; } | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。 |
| [CreatedTime](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/createdtime/) { get; set; } | 获取和设置生成 pdf 文档的时间。 |
| [CustomPropertiesExport](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/custompropertiesexport/) { get; set; } | 获取或设置决定导出到 PDF 文件方式的值。默认值为 None。 |
| [DisplayDocTitle](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/displaydoctitle/) { get; set; } | 指示窗口标题栏是否应显示文档标题。 |
| [EmbedStandardWindowsFonts](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/embedstandardwindowsfonts/) { get; set; } | 设置为 true 以嵌入 TrueType 字体。仅影响 ASCII 字符 32-127。字符代码大于 127 的字体始终嵌入。对于 PDF/A-1a、PDF/A-1b 标准，字体始终嵌入。默认值为 true。 |
| [EmfRenderSetting](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/emfrendersetting/) { get; set; } | 用于渲染 Emf 元文件的设置。 |
| [ExportDocumentStructure](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/exportdocumentstructure/) { get; set; } | 指示是否导出文档结构。 |
| [FontEncoding](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/fontencoding/) { get; set; } | 获取或设置 pdf 中嵌入的字体编码。 |
| [MergeAreas](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/mergeareas/) { get; set; } | 指示是否在保存文件之前合并条件格式和验证的区域。 |
| [OptimizationType](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/optimizationtype/) { get; set; } | 获取并设置 pdf 优化类型。 |
| [PdfCompression](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/pdfcompression/) { get; set; } | 指示压缩算法 |
| [Producer](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/producer/) { get; set; } | 获取并设置生成的 pdf 文档的生产者。 |
| [RefreshChartCache](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/refreshchartcache/) { get; set; } | 指示是否刷新图表缓存数据 |
| [SortExternalNames](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/sortexternalnames/) { get; set; } | 指示是否在保存文件前对外部已定义的名称进行排序。 |
| [SortNames](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/sortnames/) { get; set; } | 指示是否在保存文件前对已定义的名称进行排序。 |
| [UpdateSmartArt](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/updatesmartart/) { get; set; } | 指示是否更新 Smart Art 设置。默认值为 false。 |
| [ValidateMergedAreas](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/validatemergedareas/) { get; set; } | 指示是否在保存文件前验证合并单元格。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [SetImageResample](../../aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/)(int, int) | 设置重新采样图像的期望 PPI(pixels per inch) 和 jpeg 质量。所有图像将按照指定的质量设置转换为 JPEG，且像素密度大于指定的 PPI(pixels per inch) 的图像将被重新采样。 |

### 另请参见

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


