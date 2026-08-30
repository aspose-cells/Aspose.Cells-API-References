---
title: Aspose::Cells::PdfSaveOptions::GetWatermark method
linktitle: GetWatermark
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::GetWatermark method. Gets or sets watermark to output in C++.'
type: docs
weight: 3300
url: /es/cpp/aspose.cells/pdfsaveoptions/getwatermark/
---
## PdfSaveOptions::GetWatermark method


Gets or sets watermark to output.

```cpp
RenderingWatermark Aspose::Cells::PdfSaveOptions::GetWatermark()
```


## Examples


```cpp
Aspose::Cells::Startup();
//El siguiente código establece una marca de agua en el pdf de salida.

//preparar un libro de trabajo con 3 páginas.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Page1");
int index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page2");
index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page3");
wb.GetWorksheets().Get(index).GetPageSetup().SetPaperSize(PaperSizeType::PaperA3);

//crear una fuente para la marca de agua y especificar negrita, cursiva, color
RenderingFont font(u"Calibri", 68);
font.SetItalic(true);
font.SetBold(true);
font.SetColor(Color{ 0xff, 0, 0, 0xff });//Blue

//crear una marca de agua a partir de texto y la fuente especificada
RenderingWatermark watermark(u"Watermark", font);

//especificar alineación horizontal y vertical
watermark.SetHAlignment(TextAlignmentType::Center);
watermark.SetVAlignment(TextAlignmentType::Center);

//especificar rotación
watermark.SetRotation(30);

//especificar opacidad
watermark.SetOpacity(0.6f);

//especificar la escala a la página (p. ej., 100, 50) en porcentaje.
watermark.SetScaleToPagePercent(50);

//especificar marca de agua para renderizar a pdf.
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
