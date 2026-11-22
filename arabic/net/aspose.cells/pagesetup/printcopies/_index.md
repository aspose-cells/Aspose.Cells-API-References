---
title: "PageSetup.PrintCopies"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تحصل وتضبط عدد النسخ للطباعة"
type: docs
url: /ar/net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

يحصل على عدد النسخ للطباعة ويضبطه.

```csharp
public int PrintCopies { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCopiesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين عدد نسخ الطباعة إلى 3
            worksheet.PageSetup.PrintCopies = 3;
            
            // عرض إعداد عدد نسخ الطباعة الحالي
            Console.WriteLine("Print Copies: " + worksheet.PageSetup.PrintCopies);
            
            // احفظ المصنف
            workbook.Save("PageSetup_PrintCopies_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


