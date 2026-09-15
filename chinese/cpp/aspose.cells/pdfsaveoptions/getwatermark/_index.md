---
title: Aspose::Cells::PdfSaveOptions::GetWatermark method
linktitle: GetWatermark
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::GetWatermark method. Gets or sets watermark to output in C++.'
type: docs
weight: 3300
url: /zh/cpp/aspose.cells/pdfsaveoptions/getwatermark/
---
## PdfSaveOptions::GetWatermark method


Gets or sets watermark to output.

```cpp
RenderingWatermark Aspose::Cells::PdfSaveOptions::GetWatermark()
```


## Examples


```cpp
Aspose::Cells::Startup();
//以下代码在输出 pdf 中设置水印。

//准备一个包含 3 页的工作簿。
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Page1");
int index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page2");
index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page3");
wb.GetWorksheets().Get(index).GetPageSetup().SetPaperSize(PaperSizeType::PaperA3);

//为水印创建字体，并指定粗体、斜体、颜色
RenderingFont font(u"Calibri", 68);
font.SetItalic(true);
font.SetBold(true);
font.SetColor(Color{ 0xff, 0, 0, 0xff });//Blue

//使用文本和指定的字体创建水印
RenderingWatermark watermark(u"Watermark", font);

//指定水平和垂直对齐方式
watermark.SetHAlignment(TextAlignmentType::Center);
watermark.SetVAlignment(TextAlignmentType::Center);

//指定旋转角度
watermark.SetRotation(30);

//指定不透明度
watermark.SetOpacity(0.6f);

//指定相对于页面的缩放比例（例如 100、50），单位为百分比。
watermark.SetScaleToPagePercent(50);

//指定用于渲染为 pdf 的水印。
PdfSaveOptions options;
if (options.GetWatermark().IsNull())
{
    options.SetWatermark(watermark);
}

wb.Save(u"output_watermark.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
