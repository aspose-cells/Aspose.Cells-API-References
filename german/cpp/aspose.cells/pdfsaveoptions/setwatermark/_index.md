---
title: Aspose::Cells::PdfSaveOptions::SetWatermark method
linktitle: SetWatermark
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::SetWatermark method. Gets or sets watermark to output in C++.'
type: docs
weight: 3400
url: /de/cpp/aspose.cells/pdfsaveoptions/setwatermark/
---
## PdfSaveOptions::SetWatermark method


Gets or sets watermark to output.

```cpp
void Aspose::Cells::PdfSaveOptions::SetWatermark(const RenderingWatermark &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Der folgende Code setzt ein Wasserzeichen im Ausgabe‑PDF.

//Ein Arbeitsbuch mit 3 Seiten vorbereiten.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Page1");
int index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page2");
index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page3");
wb.GetWorksheets().Get(index).GetPageSetup().SetPaperSize(PaperSizeType::PaperA3);

//Erstellen Sie eine Schriftart für das Wasserzeichen und geben Sie fett, kursiv und Farbe an.
RenderingFont font(u"Calibri", 68);
font.SetItalic(true);
font.SetBold(true);
font.SetColor(Color{ 0xff, 0, 0, 0xff });//Blue

//Erstellen Sie ein Wasserzeichen aus Text und der angegebenen Schriftart.
RenderingWatermark watermark(u"Watermark", font);

//Horizontale und vertikale Ausrichtung festlegen
watermark.SetHAlignment(TextAlignmentType::Center);
watermark.SetVAlignment(TextAlignmentType::Center);

//Drehung festlegen
watermark.SetRotation(30);

//Deckkraft festlegen
watermark.SetOpacity(0.6f);

//Skalierung zur Seite (z. B. 100, 50) in Prozent festlegen.
watermark.SetScaleToPagePercent(50);

//Wasserzeichen für die PDF‑Erstellung festlegen.
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
