---
title: "تعداد HtmlCrossType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.HtmlCrossType. يمثل خمسة أنواع من سلاسل تقاطع html"
type: docs
url: /ar/net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

يمثل خمسة أنواع من سلاسل HTML المتقاطعة.

```csharp
public enum HtmlCrossType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` | العرض مثل MS Excel، يعتمد على الخلية التالية. إذا كانت الخلية التالية فارغة، ستتقاطع السلسلة، أو سيتم قطعها |
| MSExport | `1` | عرض السلسلة مثل MS Excel عند تصدير html. |
| Cross | `2` | عرض سلسلة تقاطع HTML، هذه الأداء لإنشاء ملفات html الكبيرة سيكون أسرع بأكثر من عشرة أضعاف مقارنةً بتعيين القيمة إلى Default أو FitToCell. |
| CrossHideRight | `3` | عرض سلسلة تقاطع HTML وإخفاء السلسلة اليمنى عندما تتداخل النصوص. |
| FitToCell | `4` | عرض السلسلة فقط ضمن عرض الخلية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHtmlCrossTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);
            
            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // تعيين نوع التقاطع إلى MSExport
            options.HtmlCrossStringType = HtmlCrossType.MSExport;
            
            // حفظ المصنف باستخدام خيارات HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with HtmlCrossType.MSExport");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


