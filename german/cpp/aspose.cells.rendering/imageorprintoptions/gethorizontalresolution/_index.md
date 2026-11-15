---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution method
linktitle: GetHorizontalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution method. Gets or sets the horizontal resolution for generated images, in dots per inch in C++.'
type: docs
weight: 800
url: /de/cpp/aspose.cells.rendering/imageorprintoptions/gethorizontalresolution/
---
## ImageOrPrintOptions::GetHorizontalResolution method


Gets or sets the horizontal resolution for generated images, in dots per inch.

```cpp
int32_t Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution()
```

## Remarks


The default value is 96.

Setting HorizontalResolution and VerticalResolution effects the width and height of the output image in pixels.

## Examples


```cpp
Aspose::Cells::Startup();
//          Der folgende Code setzt die Auflösung auf 192, die Breite und Höhe des erzeugten Bildes sind das Doppelte von
//          derjenigen mit der Auflösung, die auf den Standardwert 96 belassen wurde.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//Setze den Ausgabetyp des Bildes: png.
opts.SetImageType(ImageType::Png);

//Setze die Auflösung auf 192.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//Rendere die Arbeitsblattseite als Bild.
SheetRender sr(wb.GetWorksheets().Get(0), opts);
sr.ToImage(0, u"Sheet_Page1.png");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
