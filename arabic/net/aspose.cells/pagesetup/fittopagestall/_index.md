---
title: "PageSetup.FitToPagesTall"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageSetup. تمثل عدد الصفحات التي سيُحجم إليها ورقة العمل عند طباعتها. القيمة الافتراضية هي 1"
type: docs
url: /ar/net/aspose.cells/pagesetup/fittopagestall/
---
## PageSetup.FitToPagesTall property

يمثل عدد الصفحات عموديًا التي سيتم تحجيم الورقة إليها عند طباعتها. القيمة الافتراضية هي 1.

```csharp
public int FitToPagesTall { get; set; }
```

### ملاحظات

يجب عليك ضبط FitToPagesWide على الصفر إذا كنت تريد ملاءمة جميع الصفوف في صفحة واحدة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFitToPagesTallDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة لجعل الورقة تمتد على عدة صفحات
            for (int i = 0; i < 100; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Row {i+1}, Col {j+1}");
                }
            }

            // احصل على كائن PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تعيين منطقة الطباعة
            pageSetup.PrintArea = "A1:J100";
            
            // عيّن خاصية FitToPagesTall لتلائم جميع الصفوف في صفحة واحدة
            pageSetup.FitToPagesTall = 1;
            
            // عيّن خاصية FitToPagesWide لتلائم جميع الأعمدة في صفحة واحدة
            pageSetup.FitToPagesWide = 1;
            
            // عيّن حجم الورق
            pageSetup.PaperSize = PaperSizeType.PaperLetter;
            
            // اطبع خطوط الشبكة
            pageSetup.PrintGridlines = true;

            // أنشئ خيارات العرض
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // أنشئ مُصدّر الورقة
            SheetRender render = new SheetRender(worksheet, options);
            
            // أخرج مقياس الصفحة
            Console.WriteLine($"Page scale: {Math.Round(render.PageScale, 2)}");
        }
    }
}
```

### انظر أيضًا

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


