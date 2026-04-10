---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution method
linktitle: GetHorizontalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution method. Gets or sets the horizontal resolution for generated images, in dots per inch in C++.'
type: docs
weight: 800
url: /es/cpp/aspose.cells.rendering/imageorprintoptions/gethorizontalresolution/
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
//          El siguiente código establece la resolución a 192, el ancho y la altura de la imagen generada son el doble de
//          el que tiene la resolución dejada como el valor predeterminado 96.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//Establecer el tipo de imagen de salida: png.
opts.SetImageType(ImageType::Png);

//Establecer la resolución a 192.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//Renderizar la página de la hoja de cálculo a imagen.
SheetRender sr(wb.GetWorksheets().Get(0), opts);
sr.ToImage(0, u"Sheet_Page1.png");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
