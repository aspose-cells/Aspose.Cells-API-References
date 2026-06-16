---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method
linktitle: SetHorizontalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method. Gets or sets the horizontal resolution for generated images, in dots per inch in C++.'
type: docs
weight: 900
url: /it/cpp/aspose.cells.rendering/imageorprintoptions/sethorizontalresolution/
---
## ImageOrPrintOptions::SetHorizontalResolution method


Gets or sets the horizontal resolution for generated images, in dots per inch.

```cpp
void Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution(int32_t value)
```

## Remarks


The default value is 96.

Setting HorizontalResolution and VerticalResolution effects the width and height of the output image in pixels.

## Examples


```cpp
Aspose::Cells::Startup();
//          Il codice seguente imposta la risoluzione a 192, la larghezza e l'altezza dell'immagine generata sono il doppio di
//          quello con la risoluzione lasciata al valore predefinito 96.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//Imposta il tipo di immagine di output: png.
opts.SetImageType(ImageType::Png);

//Imposta la risoluzione a 192.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//Renderizza la pagina del foglio di lavoro in immagine.
SheetRender sr(wb.GetWorksheets().Get(0), opts);
sr.ToImage(0, u"Sheet_Page1.png");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
