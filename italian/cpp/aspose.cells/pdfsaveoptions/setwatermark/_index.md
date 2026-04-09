---
title: Aspose::Cells::PdfSaveOptions::SetWatermark method
linktitle: SetWatermark
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::SetWatermark method. Gets or sets watermark to output in C++.'
type: docs
weight: 3400
url: /it/cpp/aspose.cells/pdfsaveoptions/setwatermark/
---
## PdfSaveOptions::SetWatermark method


Gets or sets watermark to output.

```cpp
void Aspose::Cells::PdfSaveOptions::SetWatermark(const RenderingWatermark &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Il codice seguente imposta la filigrana nel PDF di output.

//prepara una cartella di lavoro con 3 pagine.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Page1");
int index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page2");
index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page3");
wb.GetWorksheets().Get(index).GetPageSetup().SetPaperSize(PaperSizeType::PaperA3);

//crea un font per la filigrana e specifica grassetto, corsivo, colore
RenderingFont font(u"Calibri", 68);
font.SetItalic(true);
font.SetBold(true);
font.SetColor(Color{ 0xff, 0, 0, 0xff });//Blue

//crea una filigrana dal testo e dal font specificato
RenderingWatermark watermark(u"Watermark", font);

//specifica l'allineamento orizzontale e verticale
watermark.SetHAlignment(TextAlignmentType::Center);
watermark.SetVAlignment(TextAlignmentType::Center);

//specifica la rotazione
watermark.SetRotation(30);

//specifica l'opacità
watermark.SetOpacity(0.6f);

//specifica la scala della pagina (ad es. 100, 50) in percentuale.
watermark.SetScaleToPagePercent(50);

//specifica la filigrana per il rendering in PDF.
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
