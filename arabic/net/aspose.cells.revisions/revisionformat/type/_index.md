---
title: "RevisionFormat.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionFormat. يحصل على نوع التنقيح"
type: docs
url: /ar/net/aspose.cells.revisions/revisionformat/type/
---
## RevisionFormat.Type property

يحصل على نوع المراجعة.

```csharp
public override RevisionType Type { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا بوضع المشاركة لتمكين تتبع المراجعات
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات وطبق التنسيق لإنشاء مراجعة
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");

            // طبق نمطًا لإنشاء مراجعة تنسيق
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);

            try
            {
                // الوصول إلى سجلات المراجعة
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // عرض قيمة خاصية Type
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);

                            // إظهار معلومات إضافية حول التنقيح
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);
                        }
                    }
                }

                // احفظ المصنف
                workbook.Save("RevisionFormatTypeDemo.xlsx");
                Console.WriteLine("Type property has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* enum [RevisionType](../../revisiontype/)
* class [RevisionFormat](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


