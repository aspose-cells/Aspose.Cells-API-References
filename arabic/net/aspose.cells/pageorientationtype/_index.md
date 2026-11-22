---
title: "تعداد PageOrientationType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.PageOrientationType. يمثل ثوابت اتجاه الطباعة"
type: docs
url: /ar/net/aspose.cells/pageorientationtype/
---
## PageOrientationType enumeration

يمثل ثوابت اتجاه الطباعة.

```csharp
public enum PageOrientationType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Landscape | `0` | اتجاه أفقي |
| Portrait | `1` | اتجاه عمودي |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageOrientationTypeDemo
    {
        public static void PageOrientationTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى في المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى كائن PageSetup في ورقة العمل
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تعيين اتجاه الصفحة إلى أفقي
            pageSetup.Orientation = PageOrientationType.Landscape;
            
            // حفظ المصنف إلى ملف
            workbook.Save("PageOrientationTypeExample_Landscape.xlsx");

            // تعيين اتجاه الصفحة إلى عمودي
            pageSetup.Orientation = PageOrientationType.Portrait;
            
            // احفظ المصنف إلى ملف مختلف
            workbook.Save("PageOrientationTypeExample_Portrait.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


