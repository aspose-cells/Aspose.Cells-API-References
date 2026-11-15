---
title: Aspose::Cells::PdfSaveOptions::SetWatermark method
linktitle: SetWatermark
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::SetWatermark method. Gets or sets watermark to output in C++.'
type: docs
weight: 3400
url: /tr/cpp/aspose.cells/pdfsaveoptions/setwatermark/
---
## PdfSaveOptions::SetWatermark method


Gets or sets watermark to output.

```cpp
void Aspose::Cells::PdfSaveOptions::SetWatermark(const RenderingWatermark &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Aşağıdaki kod, çıktı pdf'ye filigran ekler.

//3 sayfalı bir çalışma kitabı hazırla.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Page1");
int index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page2");
index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page3");
wb.GetWorksheets().Get(index).GetPageSetup().SetPaperSize(PaperSizeType::PaperA3);

//filigran için bir yazı tipi oluştur ve kalın, italik, renk belirle
RenderingFont font(u"Calibri", 68);
font.SetItalic(true);
font.SetBold(true);
font.SetColor(Color{ 0xff, 0, 0, 0xff });//Blue

//metinden ve belirtilen yazı tipinden bir filigran oluştur
RenderingWatermark watermark(u"Watermark", font);

//yatay ve dikey hizalamayı belirt
watermark.SetHAlignment(TextAlignmentType::Center);
watermark.SetVAlignment(TextAlignmentType::Center);

//döndürmeyi belirt
watermark.SetRotation(30);

//opaklığı belirt
watermark.SetOpacity(0.6f);

//Sayfaya ölçeği yüzde olarak belirtin (ör. 100, 50).
watermark.SetScaleToPagePercent(50);

//PDF'ye render için filigran belirtin.
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
