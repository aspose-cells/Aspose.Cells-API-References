---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::SetVerticalResolution method
linktitle: SetVerticalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::SetVerticalResolution method. Gets or sets the vertical resolution for generated images, in dots per inch in C++.'
type: docs
weight: 1100
url: /ar/cpp/aspose.cells.rendering/imageorprintoptions/setverticalresolution/
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
//          الكود التالي يضبط الدقة إلى 192، وعرض وارتفاع الصورة المولدة هو ضعف
//          الواحد الذي ترك الدقة كقيمة افتراضية 96.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//تعيين نوع صورة الإخراج: png.
opts.SetImageType(ImageType::Png);

//تعيين الدقة إلى 192.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//تحويل المخطط إلى صورة.
wb.GetWorksheets().Get(0).GetCharts().Get(0).ToImage(u"Chart.png", opts);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
