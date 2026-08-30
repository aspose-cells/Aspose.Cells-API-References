---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method
linktitle: SetHorizontalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method. Gets or sets the horizontal resolution for generated images, in dots per inch in C++.'
type: docs
weight: 900
url: /ru/cpp/aspose.cells.rendering/imageorprintoptions/sethorizontalresolution/
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
//          The following code sets resolution to 192, the width and height of the generated image is twice of
//          тот, у которого разрешение оставлено со значением по умолчанию 96.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//Установите тип выходного изображения: png.
opts.SetImageType(ImageType::Png);

//Установите разрешение на 192.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//Отобразите страницу листа в изображение.
SheetRender sr(wb.GetWorksheets().Get(0), opts);
sr.ToImage(0, u"Sheet_Page1.png");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
