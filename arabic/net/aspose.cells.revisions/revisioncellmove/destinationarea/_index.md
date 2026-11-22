---
title: "RevisionCellMove.DestinationArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellMove. تحصل على المنطقة الوجهة"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellmove/destinationarea/
---
## RevisionCellMove.DestinationArea property

يحصل على المنطقة الوجهة.

```csharp
public CellArea DestinationArea { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionCellMovePropertyDestinationAreaDemo
    {
        public static void Run()
        {
            // إنشاء مصنف للحصول على بيئة صالحة (اختياري للعرض)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Demo";

            try
            {
                // إنشاء نسخة من RevisionCellMove عبر الانعكاس (منشئ بدون معلمات)
                RevisionCellMove revMove = (RevisionCellMove)Activator.CreateInstance(typeof(RevisionCellMove));

                // قراءة وعرض خاصية DestinationArea (للقراءة فقط)
                CellArea destination = revMove.DestinationArea;
                Console.WriteLine("DestinationArea: " + destination.ToString());

                // سياق إضافي (اختياري)
                Console.WriteLine("SourceArea: " + revMove.SourceArea.ToString());
                Console.WriteLine("Revision Type: " + revMove.Type);

                // حفظ المصنف (اختياري)
                workbook.Save("RevisionCellMoveDestinationAreaDemo.xlsx");
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


