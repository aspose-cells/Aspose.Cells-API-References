---
title: "PageSetup.PrintTitleRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل الصفوف التي تحتوي على الخلايا التي يجب تكرارها في أعلى كل صفحة"
type: docs
url: /ar/net/aspose.cells/pagesetup/printtitlerows/
---
## PageSetup.PrintTitleRows property

يمثل الصفوف التي تحتوي على الخلايا التي ستُكرر في أعلى كل صفحة.

```csharp
public string PrintTitleRows { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleRowsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بتعيين بعض البيانات النموذجية
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Data " + (i-1));
            }
            
            // الوصول إلى إعداد الصفحة
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تعيين صفوف عنوان الطباعة (سيتم تكرار الصف الأول في كل صفحة مطبوعة)
            pageSetup.PrintTitleRows = "$1:$1";
            
            // احفظ المصنف
            workbook.Save("PrintTitleRowsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


