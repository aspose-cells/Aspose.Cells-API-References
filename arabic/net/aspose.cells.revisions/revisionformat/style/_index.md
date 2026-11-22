---
title: "RevisionFormat.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionFormat. يحصل على النمط المطبق"
type: docs
url: /ar/net/aspose.cells.revisions/revisionformat/style/
---
## RevisionFormat.Style property

يحصل على النمط المطبق.

```csharp
public Style Style { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد (يتم تمكين تتبع الإصدارات بشكل افتراضي عند إجراء تغييرات)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات والتنسيق لإنشاء تنقيح
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Original Value");
            
            // إنشاء نمط وتطبيقه على الخلية
            Style originalStyle = workbook.CreateStyle();
            originalStyle.Font.Name = "Arial";
            originalStyle.Font.Size = 12;
            originalStyle.Font.IsBold = true;
            cell.SetStyle(originalStyle);

            // الوصول إلى التنقيحات عبر RevisionLogs
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                RevisionCollection revisions = revisionLog.Revisions;
                foreach (Revision revision in revisions)
                {
                    if (revision is RevisionFormat revisionFormat)
                    {
                        // عرض خصائص النمط الحالية من التنقيح
                        Style style = revisionFormat.Style;
                        Console.WriteLine("Revision Style Font: " + style.Font.Name);
                        Console.WriteLine("Revision Style Font Size: " + style.Font.Size);
                        Console.WriteLine("Revision Style Is Bold: " + style.Font.IsBold);

                        // ملاحظة: خاصية النمط للقراءة فقط في RevisionFormat، لذلك لا يمكننا تعديلها مباشرة
                        // لتغيير التنسيق، سنحتاج إلى تعديل نمط الخلية مباشرة
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionFormatStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../../aspose.cells/style/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


