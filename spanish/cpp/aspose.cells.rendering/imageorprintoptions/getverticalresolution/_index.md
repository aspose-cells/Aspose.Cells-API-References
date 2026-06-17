---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::GetVerticalResolution method
linktitle: GetVerticalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::GetVerticalResolution method. Gets or sets the vertical resolution for generated images, in dots per inch in C++.'
type: docs
weight: 1000
url: /es/cpp/aspose.cells.rendering/imageorprintoptions/getverticalresolution/
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
//          El siguiente código establece la resolución a 192, el ancho y la altura de la imagen generada son el doble de
//          el que tiene la resolución dejada como el valor predeterminado 96.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//Establecer el tipo de imagen de salida: png.
opts.SetImageType(ImageType::Png);

//Establecer la resolución a 192.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//Renderizar el gráfico a imagen.
wb.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(u"Chart.png", opts);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
