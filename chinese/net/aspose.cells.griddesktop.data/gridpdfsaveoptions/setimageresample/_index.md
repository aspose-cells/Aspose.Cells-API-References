---
title: "GridPdfSaveOptions.SetImageResample"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "GridPdfSaveOptions 方法。设置重新采样图像的期望 PPI（每英寸像素）和 JPEG 质量。所有图像将转换为 JPEG，使用指定的质量设置，且像素密度高于指定 PPI 的图像将被重新采样"
type: docs
url: /zh/net/aspose.cells.griddesktop.data/gridpdfsaveoptions/setimageresample/
---
## GridPdfSaveOptions.SetImageResample method

设置重新采样图像的期望 PPI(pixels per inch) 和 jpeg 质量。所有图像将按照指定的质量设置转换为 JPEG，且像素密度大于指定的 PPI(pixels per inch) 的图像将被重新采样。

```csharp
public void SetImageResample(int desiredPPI, int jpegQuality)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| desiredPPI | Int32 | 期望的每英寸像素。220 为高质量。150 为屏幕质量。96 为邮件质量。 |
| jpegQuality | Int32 | 0 - 100% JPEG 质量。 |

### 示例

以下代码将输出 PDF 中图像的期望 PPI 设置为 96，JPEG 质量设置为 80。

```csharp
//加载带有图像的源文件。
Workbook wb = new Workbook("Book1.xlsx");

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

//将期望 PPI 设置为 96，JPEG 质量设置为 80。
pdfSaveOptions.SetImageResample(96, 80);

wb.Save("output.pdf", pdfSaveOptions);
```

### 另请参见

* class [GridPdfSaveOptions](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


