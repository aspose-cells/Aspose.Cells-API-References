---
title: "RevisionCellMove.SourceArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellMove. تحصل على المنطقة المصدر"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellmove/sourcearea/
---
## RevisionCellMove.SourceArea property

يحصل على المنطقة المصدر.

```csharp
public CellArea SourceArea { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCellMovePropertySourceAreaDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض الخلايا ببيانات عينة
            worksheet.Cells["A1"].Value = "First";
            worksheet.Cells["A2"].Value = "Second";
            worksheet.Cells["A3"].Value = "Third";

            try
            {
                // -------------------------------------------------------------
                // العينة الأصلية استخدمت ميزات تتبع التعديلات التي ليست
                // جزءًا من API المنعكس (IsTrackChanges, MoveRows, Revisions).
                // للحفاظ على جاهزية الكود للتجميع نوضح خاصية SourceArea
                // الخاصية بإنشاء مثيل من RevisionCellMove عبر الانعكاس.
                // -------------------------------------------------------------

                // إنشاء مثيل من RevisionCellMove باستخدام الانعكاس
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // عرض قيمة SourceArea (للقراءة فقط)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea.ToString());

                // معلومات إضافية ذات صلة (اختياري)
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea.ToString());

                // قد تكون SourceWorksheet فارغة (null) لنسخة تم إنشاؤها حديثًا
                if (cellMoveRev.SourceWorksheet != null)
                    Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet.Name);
                else
                    Console.WriteLine("SourceWorksheet: null");

                // احفظ دفتر العمل (اختياري)
                workbook.Save("RevisionCellMoveSourceAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


