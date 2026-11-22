---
title: "RevisionCellChange.IsNewFormatted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellChange. تشير إلى ما إذا كانت هذه الخلية مُنسقة حديثًا"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellchange/isnewformatted/
---
## RevisionCellChange.IsNewFormatted property

يشير إلى ما إذا كانت هذه الخلية مُنسقة حديثًا.

```csharp
public bool IsNewFormatted { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsNewFormattedDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين قيمة الخلية الأولية والنمط
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Initial Value");
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            cell.SetStyle(initialStyle);

            // تغيير قيمة الخلية والنمط لإنشاء مراجعة
            cell.PutValue("Updated Value");
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Calibri";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);

            // الوصول إلى سجلات المراجعة
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // عرض معلومات المراجعة
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Value: " + cellChange.OldValue);
                        Console.WriteLine("New Value: " + cellChange.NewValue);

                        // إظهار خاصية IsNewFormatted
                        Console.WriteLine("\nFormatting Information:");
                        Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);
                        Console.WriteLine("IsNewFormatted: " + cellChange.IsNewFormatted);

                        if (cellChange.IsNewFormatted)
                        {
                            Console.WriteLine("The cell has new formatting applied in this revision.");
                            Console.WriteLine("New Font: " + cellChange.NewStyle.Font.Name);
                            Console.WriteLine("New Font Size: " + cellChange.NewStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + cellChange.NewStyle.Font.IsBold);
                        }
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCellChangePropertyIsNewFormattedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


