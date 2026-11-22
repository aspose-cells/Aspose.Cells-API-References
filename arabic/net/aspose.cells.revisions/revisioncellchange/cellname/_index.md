---
title: "RevisionCellChange.CellName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellChange. تحصل على اسم الخلية"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellchange/cellname/
---
## RevisionCellChange.CellName property

يحصل على اسم الخلية.

```csharp
public string CellName { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyCellNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات أولية لإنشاء مراجعة
            worksheet.Cells["A1"].PutValue("Original Value");

            // تعديل الخلية لإنشاء مراجعة
            worksheet.Cells["A1"].PutValue("Modified Value");

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
                            // عرض قيمة الخاصية CellName
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);

                            // إظهار كيفية استخدام الخاصية CellName
                            if (cellChange.CellName == "A1")
                            {
                                Console.WriteLine("\nThe revision is for cell A1");
                                Console.WriteLine("Old Value: " + cellChange.OldValue);
                                Console.WriteLine("New Value: " + cellChange.NewValue);
                            }
                        }
                    }
                }

                // احفظ المصنف
                workbook.Save("RevisionCellChangePropertyCellNameDemo.xlsx");
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


