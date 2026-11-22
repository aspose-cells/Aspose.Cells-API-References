---
title: "LoadOptions.SetPaperSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LoadOptions. تحدد حجم ورق الطباعة الافتراضي من إعدادات الطابعات الافتراضية"
type: docs
url: /ar/net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

يضبط حجم ورق الطباعة الافتراضي من إعدادات الطابعة الافتراضية.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | PaperSizeType | حجم الورق الافتراضي. |

### ملاحظات

إذا لم يكن هناك إعداد لحجم الورق، سيستخدم MS Excel إعداد الطابعة الافتراضية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsMethodSetPaperSizeWithPaperSizeTypeDemo
    {
        public static void Run()
        {
            // إنشاء خيارات التحميل وتعيين حجم الورق إلى A5
            LoadOptions options = new LoadOptions();
            options.SetPaperSize(PaperSizeType.PaperA5);

            // تحميل دفتر العمل باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("example.xlsx", options);
            
            // تحقق من أن حجم الورق تم تعيينه بشكل صحيح
            Console.WriteLine("Paper size of first worksheet: " + workbook.Worksheets[0].PageSetup.PaperSize);
        }
    }
}
```

### انظر أيضًا

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


