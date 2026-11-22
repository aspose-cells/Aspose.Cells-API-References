---
title: "PageStartSavingArgs.IsToOutput"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PageStartSavingArgs. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب إخراج الصفحة. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells.rendering/pagestartsavingargs/istooutput/
---
## PageStartSavingArgs.IsToOutput property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب إخراج الصفحة. القيمة الافتراضية هي true.

```csharp
public bool IsToOutput { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageStartSavingArgsPropertyIsToOutputDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ البيانات لإنشاء صفحات متعددة
            for (int i = 0; i < 100; i++)
            {
                worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
                // تم التصحيح: الوصول إلى ارتفاع الصف عبر مجموعة Rows في ورقة العمل
                worksheet.Cells.Rows[i].Height = 50;
            }

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new CustomPageSavingCallback();

            workbook.Save("PageOutputDemo.pdf", saveOptions);
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                // قراءة القيمة الحالية
                Console.WriteLine($"Page {args.PageIndex + 1} - Initial IsToOutput: {args.IsToOutput}");

                // تخطي كل صفحة ذات رقم زوجي (ترقيم يبدأ من 1)
                if ((args.PageIndex + 1) % 2 == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine($"Disabling output for page {args.PageIndex + 1}");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                // لا يلزم تنفيذ ذلك لهذا العرض
            }
        }
    }
}
```

### انظر أيضًا

* class [PageStartSavingArgs](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


