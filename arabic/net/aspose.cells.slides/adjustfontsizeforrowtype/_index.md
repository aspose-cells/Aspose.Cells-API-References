---
title: "تعداد AdjustFontSizeForRowType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Slides.AdjustFontSizeForRowType. يمثل نوع الصفوف التي يجب تعديل حجم الخط لها"
type: docs
url: /ar/net/aspose.cells.slides/adjustfontsizeforrowtype/
---
## AdjustFontSizeForRowType enumeration

يمثل أي نوع من الصفوف يجب تعديلها.

```csharp
public enum AdjustFontSizeForRowType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون تعديل. |
| EmptyRows | `1` | إذا كان الصف فارغًا، غيّر حجم الخط ليتناسب مع ارتفاع الصف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassAdjustFontSizeForRowTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات في ورقة العمل
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // إنشاء نسخة من PptxSaveOptions مع إعداد AdjustFontSizeForRowType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                AdjustFontSizeForRowType = AdjustFontSizeForRowType.EmptyRows
            };

            // حفظ المصنف كملف PPTX
            workbook.Save("AdjustFontSizeForRowTypeDemo.pptx", saveOptions);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


