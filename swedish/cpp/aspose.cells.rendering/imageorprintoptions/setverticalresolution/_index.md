---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::SetVerticalResolution method
linktitle: SetVerticalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::SetVerticalResolution method. Gets or sets the vertical resolution for generated images, in dots per inch in C++.'
type: docs
weight: 1100
url: /sv/cpp/aspose.cells.rendering/imageorprintoptions/setverticalresolution/
---
## ImageOrPrintOptions::SetVerticalResolution method


Gets or sets the vertical resolution for generated images, in dots per inch.

```cpp
void Aspose::Cells::Rendering::ImageOrPrintOptions::SetVerticalResolution(int32_t value)
```

## Remarks


The default value is 96.

Setting HorizontalResolution and VerticalResolution effects the width and height of the output image in pixels.

## Examples


```cpp
Aspose::Cells::Startup();
//          Följande kod sätter upplösningen till 192, bredden och höjden på den genererade bilden är dubbelt så stor som
//          den med upplösning kvar som standardvärde 96.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//Ställ in utdata bildtyp: png.
opts.SetImageType(ImageType::Png);

//Ställ in upplösning till 192.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//Rendera diagram till bild.
wb.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(u"Chart.png", opts);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
