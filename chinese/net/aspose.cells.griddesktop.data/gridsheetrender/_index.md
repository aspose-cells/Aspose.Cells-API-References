---
title: "类 GridSheetRender"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridDesktop.Data.GridSheetRender 类。表示一个工作表渲染器，可将工作表渲染为 BMP、PNG、JPEG、TIFF 等多种图像。此类的构造函数必须在修改页面设置和单元格样式后使用。"
type: docs
url: /zh/net/aspose.cells.griddesktop.data/gridsheetrender/
---
## GridSheetRender class

表示一个工作表渲染器，可将工作表渲染为 (BMP、PNG、JPEG、TIFF…) 等多种图像。此类的构造函数必须在修改页面设置和单元格样式后使用。

```csharp
public class GridSheetRender
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GridSheetRender](gridsheetrender/)(Worksheet, GridImageOrPrintOptions) | SheetRender 的构造函数，需要工作表和 ImageOrPrintOptions 作为参数 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [PageCount](../../aspose.cells.griddesktop.data/gridsheetrender/pagecount/) { get; } | 获取当前工作表的总页数。 |
| [PageScale](../../aspose.cells.griddesktop.data/gridsheetrender/pagescale/) { get; } | 获取工作表的计算页面比例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetPageSizeInch](../../aspose.cells.griddesktop.data/gridsheetrender/getpagesizeinch/)(int) | 获取输出图像的页面尺寸（英寸）。 |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage)(int) | 将指定页面渲染为 Bitmap 对象。 |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_3)(int, Stream) | 将指定页面渲染到流中。 |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_4)(int, string) | 将指定页面渲染到文件中。 |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_1)(int, Graphics, float, float) | 将指定页面渲染到 Graphics。 |
| [ToImage](../../aspose.cells.griddesktop.data/gridsheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | 将指定页面渲染到 Graphics。 |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter)(PrinterSettings) | 将工作表渲染到打印机 |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_2)(string) | 将工作表渲染到打印机 |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | 将工作表渲染到打印机 |
| [ToPrinter](../../aspose.cells.griddesktop.data/gridsheetrender/toprinter/#toprinter_3)(string, string) | 将工作表渲染到打印机 |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff)(Stream) | 将整个工作表渲染为 Tiff 图像并输出到流。 |
| [ToTiff](../../aspose.cells.griddesktop.data/gridsheetrender/totiff/#totiff_1)(string) | 将整个工作表渲染为 Tiff 图像并保存到文件。 |

### 另请参见

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


