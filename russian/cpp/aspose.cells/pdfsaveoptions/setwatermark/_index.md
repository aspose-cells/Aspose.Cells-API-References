---
title: Aspose::Cells::PdfSaveOptions::SetWatermark method
linktitle: SetWatermark
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::SetWatermark method. Gets or sets watermark to output in C++.'
type: docs
weight: 3400
url: /ru/cpp/aspose.cells/pdfsaveoptions/setwatermark/
---
## PdfSaveOptions::SetWatermark method


Gets or sets watermark to output.

```cpp
void Aspose::Cells::PdfSaveOptions::SetWatermark(const RenderingWatermark &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Следующий код устанавливает водяной знак в выходном PDF.

//подготовить рабочую книгу с 3 страницами.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Page1");
int index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page2");
index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page3");
wb.GetWorksheets().Get(index).GetPageSetup().SetPaperSize(PaperSizeType::PaperA3);

//создать шрифт для водяного знака и указать полужирный, курсив, цвет
RenderingFont font(u"Calibri", 68);
font.SetItalic(true);
font.SetBold(true);
font.SetColor(Color{ 0xff, 0, 0, 0xff });//Blue

//создать водяной знак из текста с указанным шрифтом
RenderingWatermark watermark(u"Watermark", font);

//указать горизонтальное и вертикальное выравнивание
watermark.SetHAlignment(TextAlignmentType::Center);
watermark.SetVAlignment(TextAlignmentType::Center);

//указать вращение
watermark.SetRotation(30);

//указать непрозрачность
watermark.SetOpacity(0.6f);

//указать масштаб относительно страницы (например, 100, 50) в процентах.
watermark.SetScaleToPagePercent(50);

//указать водяной знак для рендеринга в PDF.
PdfSaveOptions options;
if (options.GetWatermark().IsNull())
{
    options.SetWatermark(watermark);
}

wb.Save(u"output_watermark.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
