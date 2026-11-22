---
title: "الفئة RevisionFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.RevisionFormat الفئة. يمثل سجل مراجعة للمعلومات حول تغيير تنسيق"
type: docs
url: /ar/net/aspose.cells.revisions/revisionformat/
---
## RevisionFormat class

يمثل سجل مراجعة لمعلومات حول تغيير تنسيق.

```csharp
public class RevisionFormat : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Areas](../../aspose.cells.revisions/revisionformat/areas/) { get; } | النطاق الذي تم تطبيق هذا التنسيق عليه. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| [Style](../../aspose.cells.revisions/revisionformat/style/) { get; } | يحصل على النمط المطبق. |
| override [Type](../../aspose.cells.revisions/revisionformat/type/) { get; } | يحصل على نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionFormatDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا بوضع المشاركة لتمكين تتبع المراجعات
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف بعض البيانات وطبق التنسيق لإنشاء مراجعة
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Sample Data");

                // طبق نمطًا لإنشاء مراجعة تنسيق
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                cell.SetStyle(style);

                // الوصول إلى سجلات المراجعة
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // عرض خصائص المراجعة
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);

                            // عرض معلومات النمط
                            Style revisionStyle = revisionFormat.Style;
                            Console.WriteLine("Font Name: " + revisionStyle.Font.Name);
                            Console.WriteLine("Font Size: " + revisionStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + revisionStyle.Font.IsBold);
                        }
                    }
                }

                // احفظ المصنف
                workbook.Save("RevisionFormatDemo.xlsx");
                Console.WriteLine("RevisionFormat demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionFormat: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


