---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::GetVerticalResolution method
linktitle: GetVerticalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::GetVerticalResolution method. Gets or sets the vertical resolution for generated images, in dots per inch in C++.'
type: docs
weight: 1000
url: /it/cpp/aspose.cells.rendering/imageorprintoptions/getverticalresolution/
---
## ImageOrPrintOptions::GetVerticalResolution method


Gets or sets the vertical resolution for generated images, in dots per inch.

```cpp
int32_t Aspose::Cells::Rendering::ImageOrPrintOptions::GetVerticalResolution()
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

//Renderizza il grafico in immagine.
wb.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(u"Chart.png", opts);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
