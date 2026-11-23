---
title: "类 GridJsOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridJs.GridJsOptions 类。表示 GridJs 的所有加载选项"
type: docs
url: /zh/net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

表示 GridJs 的所有加载选项

```csharp
public class GridJsOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitcolumnsonload/) { get; set; } | 指示在加载文件时是否自动调整列宽，默认值为 false。 |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | 指示在加载文件时是否自动调整行高，默认值为 false。 |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | 获取/设置是否自动优化包含大单元格的工作表的加载性能。它将忽略某些样式/边框以减少加载时间。默认值为 true。 |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | 获取/设置 GridJs 控制器的路由 URL 基础名称。默认是 GridJs2 |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | 获取/设置 PDF 导出使用的自定义 PdfSaveOptions。如果设置，则会替代默认选项。默认值为 null。 |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | 获取/设置 空工作表的默认最大列数。默认值为 15。 |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | 获取/设置 空工作表的默认最大行数。默认值为 12。 |
| [EnableChartClientRendering](../../aspose.cells.gridjs/gridjsoptions/enablechartclientrendering/) { get; set; } | 获取/设置 是否启用客户端图表渲染。如果设为 false，GridJs 将仅输出图表图像/形状，不需要客户端图表渲染。默认值为 true。 |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | 获取/设置 用于存储电子表格文件的缓存目录。我们需要在使用 GridJs 之前将其设置为特定路径。 |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | 获取/设置 渲染图片/形状中使用的字体文件夹 |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | 获取/设置 是否显示包含数据、样式、合并单元格和形状的最大范围。如果最后一行或列的单元格没有值和公式但具有自定义样式，则在此值为 true 时我们不会显示该行/列。默认值为 true。 |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | 获取/设置 是否支持协作编辑，默认是 false。 |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | 获取/设置 是否限制单个工作表中显示的形状/图像总数。如果设为 true，GridJs 将把单个工作表中显示的形状或图像总数限制为 MaxShapeOrImageCount。默认值为 true。 |
| [IsWasm](../../aspose.cells.gridjs/gridjsoptions/iswasm/) { get; set; } | 获取/设置 GridJs 是否在浏览器 WebAssembly 主机中运行，而不是在服务器进程中。为 true 时，不使用 FileCacheDirectory / 磁盘 / 中断线程路径，文件缓存必须来自 CacheImp，因为浏览器主机没有本地磁盘。它在运行时选择代码路径，因此同一个 Aspose.Cells.GridJs.dll 可服务于两种主机。默认值为 false。 |
| [JsonCache](../../aspose.cells.gridjs/gridjsoptions/jsoncache/) { get; set; } | 获取/设置 JSON 缓存配置选项。控制生成的工作簿 JSON 的内存 (L1) 和磁盘 (L2) 缓存行为。 |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | 获取/设置 是否仅加载活动工作表，默认是 false。 |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | 获取/设置 保存为 PDF 时的最大超时时间（秒）。默认值为 10。 |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | 获取/设置 活动工作表中显示的形状或图像的总数，IslimitShapeOrImage 为 true 时生效。默认值为 100。 |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | 获取/设置 形状或图像的最大宽度或高度，GridJs 将忽略宽度或高度大于此值的形状或图像，IslimitShapeOrImage 为 true 时生效。默认值为 10000。 |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | 获取/设置 工作簿中显示的形状或图像的总数，IslimitShapeOrImage 为 true 时生效。默认值为 300。 |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | 获取/设置 以 "/topic" 为前缀的 WebSocket 目标。默认是 "/topic/opr"。仅在协作模式下使用。 |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | 获取/设置 图片的缓存目录。（当 GridJsWorkbook.CacheImp 为 null 时生效）默认路径为 FileCacheDirectory 内的 "_piccache"。 |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | 获取/设置 是否检查图像是否具有相同来源，默认是 true，默认值为 true。 |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | 获取/设置 是否将 HTML 文件保存为 zip 压缩包，默认是 false。 |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | 获取/设置 是否显示图表工作表。默认值为 false。 |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | 获取/设置 是否跳过对 UI 不可见的形状，默认值为 true。 |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | 获取/设置 当工作表具有 PageSetup 的 PrintArea 设置时，是否在 UI 显示范围使用 PageSetup.PrintArea。默认值为 false。 |

## 字段

| 名称 | 描述 |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | 缓存存储的自定义实现，如果希望以流方式存储缓存，需要进行设置和实现。WebAssembly 主机（IsWasm = true）必须设置它，因为默认文件缓存没有本地磁盘。 |
| [RedactionUseClientGenerateId](../../aspose.cells.gridjs/gridjsoptions/redactionuseclientgenerateid/) | 指示是否在与编辑相关的操作中使用客户端生成的 ID 而不是实际的形状 ID |

### 另请参见

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


