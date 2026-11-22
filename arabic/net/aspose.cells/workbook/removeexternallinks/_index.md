---
title: "Workbook.RemoveExternalLinks"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تزيل جميع الروابط الخارجية في المصنف"
type: docs
url: /ar/net/aspose.cells/workbook/removeexternallinks/
---
## Workbook.RemoveExternalLinks method

يزيل جميع الروابط الخارجية في المصنف.

```csharp
[Obsolete("Use ExternalLinkCollection.Clear() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void RemoveExternalLinks()
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة ExternalLinkCollection.Clear(). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ ديسمبر 2021. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodRemoveExternalLinksDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للسياق
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // استدعاء طريقة RemoveExternalLinks
                workbook.RemoveExternalLinks();

                // عرض النتائج أو تأثيرات استدعاء الطريقة
                Console.WriteLine("RemoveExternalLinks method called successfully");

                // احفظ المصنف إذا تم إجراء تغييرات
                workbook.Save("RemoveExternalLinksDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling RemoveExternalLinks: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


