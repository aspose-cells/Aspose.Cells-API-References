---
title: Aspose::Cells::PdfSaveOptions::SetWatermark method
linktitle: SetWatermark
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::SetWatermark method. Gets or sets watermark to output in C++.'
type: docs
weight: 3400
url: /ar/cpp/aspose.cells/pdfsaveoptions/setwatermark/
---
## PdfSaveOptions::SetWatermark method


Gets or sets watermark to output.

```cpp
void Aspose::Cells::PdfSaveOptions::SetWatermark(const RenderingWatermark &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//الكود التالي يحدد علامة مائية في ملف PDF الناتج.

//تحضير دفتر عمل يحتوي على 3 صفحات.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Page1");
int index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page2");
index = wb.GetWorksheets().Add();
wb.GetWorksheets().Get(index).GetCells().Get(u"A1").PutValue(u"Page3");
wb.GetWorksheets().Get(index).GetPageSetup().SetPaperSize(PaperSizeType::PaperA3);

//إنشاء خط للعلامة المائية وتحديد الغامق والمائل واللون
RenderingFont font(u"Calibri", 68);
font.SetItalic(true);
font.SetBold(true);
font.SetColor(Color{ 0xff, 0, 0, 0xff });//Blue

//إنشاء علامة مائية من النص والخط المحدد
RenderingWatermark watermark(u"Watermark", font);

//تحديد المحاذاة الأفقية والعمودية
watermark.SetHAlignment(TextAlignmentType::Center);
watermark.SetVAlignment(TextAlignmentType::Center);

//تحديد الدوران
watermark.SetRotation(30);

//تحديد الشفافية
watermark.SetOpacity(0.6f);

//تحديد المقياس للصفحة (مثال: 100، 50) بالنسبة المئوية.
watermark.SetScaleToPagePercent(50);

//تحديد العلامة المائية للتصوير إلى PDF.
PdfSaveOptions options;
if (options.GetWatermark().IsNull())
{
    options.SetWatermark(watermark);
}

wb.Save(u"output_watermark.pdf", options);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [RenderingWatermark](../../../aspose.cells.rendering/renderingwatermark/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
