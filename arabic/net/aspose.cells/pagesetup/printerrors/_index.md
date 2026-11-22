---
title: "PageSetup.PrintErrors"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تحدد نوع خطأ الطباعة المعروض"
type: docs
url: /ar/net/aspose.cells/pagesetup/printerrors/
---
## PageSetup.PrintErrors property

يحدد نوع خطأ الطباعة المعروض.

```csharp
public PrintErrorsType PrintErrors { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintErrorsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // ضبط أخطاء الطباعة لتظهر كفراغ
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            Console.WriteLine("PrintErrors set to: " + sheet.PageSetup.PrintErrors);
            
            // تغيير أخطاء الطباعة لتظهر كشرطات
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            Console.WriteLine("PrintErrors changed to: " + sheet.PageSetup.PrintErrors);
            
            // احفظ المصنف
            workbook.Save("PrintErrorsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


