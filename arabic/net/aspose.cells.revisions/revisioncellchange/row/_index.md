---
title: "RevisionCellChange.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellChange. تحصل على فهرس الصف للخلية"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellchange/row/
---
## RevisionCellChange.Row property

يحصل على فهرس الصف للخلية.

```csharp
public int Row { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات أولية لإنشاء مراجعة
            worksheet.Cells["B5"].PutValue("Original Value");

            // تعديل الخلية لإنشاء مراجعة
            worksheet.Cells["B5"].PutValue("Modified Value");

            try
            {
                // الوصول إلى سجلات المراجعة
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // اعرض قيمة خاصية Row
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // إظهار كيفية استخدام الخاصية Row
                            if (cellChange.Row >= 0)
                            {
                                Console.WriteLine("\nThe revision occurred in row " +
                                    (cellChange.Row + 1) + " (1-based index)");
                            }
                        }
                    }
                }

                // احفظ المصنف
                workbook.Save("RevisionCellChangePropertyRowDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


