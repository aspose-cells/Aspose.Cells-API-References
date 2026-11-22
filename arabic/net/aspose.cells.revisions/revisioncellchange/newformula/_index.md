---
title: "RevisionCellChange.NewFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellChange. يحصل على الصيغة القديمة"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellchange/newformula/
---
## RevisionCellChange.NewFormula property

يحصل على الصيغة القديمة.

```csharp
public string NewFormula { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyNewFormulaDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين الصيغة الأولية في الخلية A1
            worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // غيّر الصيغة لإنشاء مراجعة
            worksheet.Cells["A1"].Formula = "=AVERAGE(B1:B3)";

            // الوصول إلى سجلات المراجعة
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // عرض معلومات تغيير الصيغة
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Formula: " + cellChange.OldFormula);
                        Console.WriteLine("New Formula: " + cellChange.NewFormula);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // توضيح استخدام خاصية NewFormula
                        if (!string.IsNullOrEmpty(cellChange.NewFormula))
                        {
                            Console.WriteLine("\nThe cell's new formula calculates: " + 
                                worksheet.Cells["A1"].StringValue);
                        }
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCellChangePropertyNewFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


