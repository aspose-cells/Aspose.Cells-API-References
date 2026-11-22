---
title: "PageSetup.FitToPagesWide"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل عدد الصفحات عرضًا التي سيُقاس إليها ورقة العمل عند طباعتها. القيمة الافتراضية هي 1"
type: docs
url: /ar/net/aspose.cells/pagesetup/fittopageswide/
---
## PageSetup.FitToPagesWide property

يمثل عدد الصفحات عرضيًا التي سيتم تحجيم الورقة إليها عند طباعتها. القيمة الافتراضية هي 1.

```csharp
public int FitToPagesWide { get; set; }
```

### ملاحظات

يجب ضبط FitToPagesTall إلى صفر إذا كنت تريد ملاءمة جميع الأعمدة في صفحة واحدة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesWideDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Sample Data 1");
            worksheet.Cells["A2"].PutValue("Sample Data 2");
            worksheet.Cells["B1"].PutValue("Sample Data 3");
            worksheet.Cells["B2"].PutValue("Sample Data 4");

            // تعيين خصائص إعداد الصفحة
            worksheet.PageSetup.FitToPagesWide = 1;  // Fit to 1 page wide
            worksheet.PageSetup.FitToPagesTall = 0; // Let height adjust automatically

            // احفظ المصنف
            workbook.Save("FitToPagesWideDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


