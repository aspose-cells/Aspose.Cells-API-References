---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method
linktitle: SetHorizontalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::SetHorizontalResolution method. Gets or sets the horizontal resolution for generated images, in dots per inch in C++.'
type: docs
weight: 900
url: /tr/cpp/aspose.cells.rendering/imageorprintoptions/sethorizontalresolution/
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
//          Aşağıdaki kod çözünürlüğü 192 olarak ayarlar, oluşturulan görüntünün genişliği ve yüksekliği iki katıdır
//          çözünürlüğü varsayılan değer 96 olarak bırakılan
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//Çıktı görüntü tipini ayarla: png.
opts.SetImageType(ImageType::Png);

//Çözünürlüğü 192 olarak ayarla.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//Çalışma sayfası sayfasını görüntüye renderla.
SheetRender sr(wb.GetWorksheets().Get(0), opts);
sr.ToImage(0, u"Sheet_Page1.png");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
