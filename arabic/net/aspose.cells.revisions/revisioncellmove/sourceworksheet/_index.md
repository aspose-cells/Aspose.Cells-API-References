---
title: "RevisionCellMove.SourceWorksheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellMove. تحصل على ورقة العمل المصدر"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellmove/sourceworksheet/
---
## RevisionCellMove.SourceWorksheet property

يحصل على ورقة العمل المصدر.

```csharp
public Worksheet SourceWorksheet { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellMovePropertySourceWorksheetDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // إنشاء مثيل من RevisionCellMove باستخدام الانعكاس
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // عرض قيمة خاصية SourceWorksheet (للقراءة فقط)
                Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet);

                // سياق إضافي (اختياري)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea);
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea);
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // احفظ دفتر العمل (اختياري)
                workbook.Save("SourceWorksheetDemo.xlsx");
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

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


