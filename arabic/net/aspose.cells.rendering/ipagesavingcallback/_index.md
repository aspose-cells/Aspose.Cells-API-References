---
title: "واجهة IPageSavingCallback"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "واجهة Aspose.Cells.Rendering.IPageSavingCallback. التحكم/الإشارة إلى تقدم عملية حفظ الصفحة"
type: docs
url: /ar/net/aspose.cells.rendering/ipagesavingcallback/
---
## IPageSavingCallback interface

التحكم/الإشارة إلى تقدم عملية حفظ الصفحة.

```csharp
public interface IPageSavingCallback
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [PageEndSaving](../../aspose.cells.rendering/ipagesavingcallback/pageendsaving/)(PageEndSavingArgs) | التحكم/الإشارة إلى انتهاء صفحة ليتم إخراجها. |
| [PageStartSaving](../../aspose.cells.rendering/ipagesavingcallback/pagestartsaving/)(PageStartSavingArgs) | التحكم/الإشارة إلى بدء صفحة ليتم إخراجها. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PageSavingCallbackDemo : IPageSavingCallback
    {
        public static void PageSavingCallbackExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");

            // إنشاء خيارات الحفظ مع رد نداء حفظ الصفحة
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.PageSavingCallback = new PageSavingCallbackDemo();

            // احفظ المصنف كملف DOCX
            workbook.Save("PageSavingCallbackExample.docx", saveOptions);
        }

        // تنفيذ طريقة PageStartSaving
        public void PageStartSaving(PageStartSavingArgs args)
        {
            Console.WriteLine($"Starting to save page {args.PageIndex}");
        }

        // تنفيذ طريقة PageEndSaving
        public void PageEndSaving(PageEndSavingArgs args)
        {
            Console.WriteLine($"Finished saving page {args.PageIndex}");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


