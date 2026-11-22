---
title: "IPageSavingCallback.PageEndSaving"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IPageSavingCallback. التحكم/الإشارة إلى انتهاء صفحة ليتم إخراجها"
type: docs
url: /ar/net/aspose.cells.rendering/ipagesavingcallback/pageendsaving/
---
## IPageSavingCallback.PageEndSaving method

التحكم/الإشارة إلى انتهاء صفحة ليتم إخراجها.

```csharp
public void PageEndSaving(PageEndSavingArgs args)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| args | PageEndSavingArgs | معلومات الصفحة تنهي عملية الحفظ. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class IPageSavingCallbackMethodPageEndSavingWithPageEndSavingArgsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد وتعبئة البيانات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لإنشاء صفحات متعددة عند العرض
            for (int i = 0; i < 500; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Row {i+1} - Demonstration data for page splitting";
            }

            // إنشاء خيارات حفظ PDF مع رد نداء مخصص لحفظ الصفحات
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.PageSavingCallback = new PageEndSavingCallback();

            try
            {
                // حفظ المصنف مع تنفيذ رد النداء
                workbook.Save("PageEndSavingDemo.pdf", saveOptions);
                Console.WriteLine("Document saved successfully with page end tracking.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during document save: {ex.Message}");
            }
        }

        private class PageEndSavingCallback : IPageSavingCallback
        {
            public void PageEndSaving(PageEndSavingArgs args)
            {
                // عرض معلومات إكمال حفظ الصفحة
                Console.WriteLine($"Finished processing page {args.PageIndex + 1}");
                
                // يمكنك إضافة عمليات ملفات أو معالجة لاحقة أخرى هنا
                // args.HasMorePages يوضح ما إذا كانت هناك صفحات إضافية سيتم معالجتها
            }

            public void PageStartSaving(PageStartSavingArgs args)
            {
                // تنفيذ الواجهة المطلوبة
            }
        }
    }
}
```

### انظر أيضًا

* class [PageEndSavingArgs](../../pageendsavingargs/)
* interface [IPageSavingCallback](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


