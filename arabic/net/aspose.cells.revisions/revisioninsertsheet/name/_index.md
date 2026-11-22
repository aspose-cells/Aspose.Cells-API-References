---
title: "RevisionInsertSheet.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionInsertSheet. تحصل على اسم ورقة العمل"
type: docs
url: /ar/net/aspose.cells.revisions/revisioninsertsheet/name/
---
## RevisionInsertSheet.Name property

يحصل على اسم ورقة العمل.

```csharp
public string Name { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertSheetPropertyNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // أضف ورقة عمل جديدة قد تولد سجل مراجعة
            Worksheet newSheet = workbook.Worksheets.Add("NewSheet");

            try
            {
                // محاكاة الوصول إلى RevisionInsertSheet من المراجعات
                // ملاحظة: في سيناريو حقيقي، سيأتي هذا من workbook.Revisions
                // للتوضيح، سننشئ سيناريو تجريبي
                RevisionInsertSheet insertSheetRevision = null;

                // في الاستخدام الفعلي، ستحصل على هذا من مجموعة المراجعات
                // على سبيل المثال: insertSheetRevision = (RevisionInsertSheet)workbook.Revisions[0];

                // نظرًا لأنه لا يمكننا إنشاء RevisionInsertSheet مباشرةً، سنوضح
                // ما الذي ستفعله إذا كان لديك إمكانية الوصول إلى واحدة
                if (insertSheetRevision != null)
                {
                    // اعرض قيمة الخاصية Name (للقراءة فقط)
                    Console.WriteLine("Inserted sheet name: " + insertSheetRevision.Name);

                    // أظهر استخدام الخاصية Name في شرط تحققي
                    if (!string.IsNullOrEmpty(insertSheetRevision.Name))
                    {
                        Console.WriteLine("The sheet has a valid name: " + insertSheetRevision.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No RevisionInsertSheet found in revisions");
                }

                // احفظ المصنف
                workbook.Save("RevisionInsertSheetNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
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

* class [RevisionInsertSheet](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


