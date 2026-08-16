---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method
linktitle: SetHorizontalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method. Gets or sets the horizontal resolution for generated images, in dots per inch in C++.'
type: docs
weight: 900
url: /de/cpp/aspose.cells.rendering/imageorprintoptions/sethorizontalresolution/
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
//          Der folgende Code setzt die Auflösung auf 192, die Breite und Höhe des erzeugten Bildes sind das Doppelte von
//          die mit Auflösung auf den Standardwert 96 belassen wurde.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//Ausgabe-Bildtyp festlegen: png.
opts.SetImageType(ImageType::Png);

//Auflösung auf 192 festlegen.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//Arbeitsblattseite als Bild rendern.
SheetRender sr(wb.GetWorksheets().Get(0), opts);
sr.ToImage(0, u"Sheet_Page1.png");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
