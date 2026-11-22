---
title: "Worksheet.GetPrintingPageBreaks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. يحصل على فواصل الصفحات التلقائية"
type: docs
url: /ar/net/aspose.cells/worksheet/getprintingpagebreaks/
---
## Worksheet.GetPrintingPageBreaks method

يحصل على فواصل الصفحات التلقائية.

```csharp
public CellArea[] GetPrintingPageBreaks(ImageOrPrintOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | ImageOrPrintOptions | خيارات الطباعة |

### قيمة الإرجاع

مناطق فواصل الصفحات التلقائية.

### ملاحظات

كل منطقة خلية تمثل ورقة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPrintingPageBreaksWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة لإنشاء فواصل الصفحات
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Row {i+1}");
            }

            // حدد منطقة الطباعة وإعداد الصفحة
            worksheet.PageSetup.PrintArea = "A1:A100";
            worksheet.PageSetup.FitToPagesTall = 1;
            worksheet.PageSetup.FitToPagesWide = 1;

            // احصل على فواصل الصفحات باستخدام ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            CellArea[] pageBreaks = worksheet.GetPrintingPageBreaks(options);

            // إخراج معلومات أول فاصل صفحة
            Console.WriteLine($"First page break ends at row: {pageBreaks[0].EndRow}");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


