---
title: Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution method
linktitle: GetHorizontalResolution
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::ImageOrPrintOptions::GetHorizontalResolution method. Gets or sets the horizontal resolution for generated images, in dots per inch in C++.'
type: docs
weight: 800
url: /ar/cpp/aspose.cells.rendering/imageorprintoptions/gethorizontalresolution/
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
//          الكود التالي يضبط الدقة إلى 192، وعرض وارتفاع الصورة المولدة هو ضعف
//          الواحد الذي ترك الدقة كقيمة افتراضية 96.
Workbook wb(u"Book1.xlsx");

ImageOrPrintOptions opts;

//تعيين نوع صورة الإخراج: png.
opts.SetImageType(ImageType::Png);

//تعيين الدقة إلى 192.
opts.SetHorizontalResolution(192);
opts.SetVerticalResolution(192);

//تحويل صفحة ورقة العمل إلى صورة.
SheetRender sr(wb.GetWorksheets().Get(0), opts);
sr.ToImage(0, u"Sheet_Page1.png");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [ImageOrPrintOptions](../)
* Namespace [Aspose::Cells::Rendering](../../)
* Library [Aspose.Cells for C++](../../../)
