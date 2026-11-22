---
title: "RevisionCellChange.IsOldFormatted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellChange. تشير إلى ما إذا كانت هذه الخلية منسقة قديمًا"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellchange/isoldformatted/
---
## RevisionCellChange.IsOldFormatted property

يشير إلى ما إذا كانت هذه الخلية مُنسقة قديمًا.

```csharp
public bool IsOldFormatted { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyIsOldFormattedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
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
                            // عرض قيمة الخاصية IsOldFormatted
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("IsOldFormatted: " + cellChange.IsOldFormatted);

                            // إظهار سياق إضافي حول المراجعة
                            if (cellChange.IsOldFormatted)
                            {
                                Console.WriteLine("The cell had formatting before this revision.");
                                Console.WriteLine("Old Font: " + cellChange.OldStyle.Font.Name);
                                Console.WriteLine("Old Font Size: " + cellChange.OldStyle.Font.Size);
                            }
                            else
                            {
                                Console.WriteLine("The cell did not have formatting before this revision.");
                            }
                        }
                    }
                }

                // احفظ المصنف مع التعديلات
                workbook.Save("IsOldFormattedDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved as IsOldFormattedDemo.xlsx");
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


