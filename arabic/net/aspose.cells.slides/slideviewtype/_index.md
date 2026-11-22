---
title: "تعداد SlideViewType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Slides.SlideViewType. يمثل النوع عند التصدير إلى الشرائح"
type: docs
url: /ar/net/aspose.cells.slides/slideviewtype/
---
## SlideViewType enumeration

يمثل النوع عند التصدير إلى الشرائح.

```csharp
public enum SlideViewType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| View | `0` | التصدير كعرض في MS Excel. |
| Print | `1` | التصدير كطباعة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slides;

namespace AsposeCellsExamples
{
    public class SlidesClassSlideViewTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Slide 1 Content");
            worksheet.Cells["A2"].PutValue("This will appear in the exported slides");

            // تكوين خيارات حفظ PPTX باستخدام SlideViewType
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                ExportViewType = SlideViewType.Print,
                OnePagePerSheet = true
            };

            // حفظ كـ PPTX
            workbook.Save("SlidesViewTypeDemo.pptx", saveOptions);
            
            Console.WriteLine("PPTX file created with SlideViewType.Print");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Slides](../../aspose.cells.slides/)
* assembly [Aspose.Cells](../../)


