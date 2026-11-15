---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::GetVerticalResolution method
linktitle: GetVerticalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::GetVerticalResolution method. Gets or sets the vertical resolution for generated images, in dots per inch in C++.'
type: docs
weight: 1000
url: /sv/cpp/aspose.cells.rendering/imageorprintoptions/getverticalresolution/
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
//          Följande kod sätter upplösningen till 192, bredden och höjden på den genererade bilden är dubbelt så stor som
//          den med upplösning som lämnas på standardvärdet 96.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//Ange bildtyp för utdata: png.
opts.SetImageType(ImageType::Png);

//Sätt upplösningen till 192.
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
