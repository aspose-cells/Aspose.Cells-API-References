---
title: "الفئة SmartTagOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Markup.SmartTagOptions. تمثل خيارات العلامة الذكية"
type: docs
url: /ar/net/aspose.cells.markup/smarttagoptions/
---
## SmartTagOptions class

يمثل خيارات العلامة الذكية.

```csharp
public class SmartTagOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SmartTagOptions](smarttagoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [EmbedSmartTags](../../aspose.cells.markup/smarttagoptions/embedsmarttags/) { get; set; } | يشير إلى ما إذا كان يتم حفظ العلامات الذكية مع المصنف. |
| [ShowType](../../aspose.cells.markup/smarttagoptions/showtype/) { get; set; } | تمثل نوع العرض للعلامة الذكية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن من SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // تعيين الخصائص
            options.EmbedSmartTags = true;
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;

            // تطبيق SmartTagOptions على ورقة العمل
            // ملاحظة: تم التغيير من worksheet.SmartTagSetting.Options = options;
            // لاستخدام كائن الخيارات مباشرةً لأن SmartTagSetting لا يحتوي على خاصية Options
            // (على افتراض أن الخيارات مقصودة للاستخدام مباشرةً)
            
            // أضف بعض البيانات للتوضيح
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);

            // احفظ المصنف
            workbook.Save("SmartTagOptionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


