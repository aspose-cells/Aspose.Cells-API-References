---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::GetVerticalResolution method
linktitle: GetVerticalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::GetVerticalResolution method. Gets or sets the vertical resolution for generated images, in dots per inch in C++.'
type: docs
weight: 1000
url: /ar/cpp/aspose.cells.rendering/imageorprintoptions/getverticalresolution/
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
