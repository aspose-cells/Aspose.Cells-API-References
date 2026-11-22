---
title: "RevisionCellChange.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellChange. تمثل نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellchange/type/
---
## RevisionCellChange.Type property

يمثل نوع المراجعة.

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

    public class RevisionCellChangePropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تمكين تتبع التغييرات عن طريق تعديل خلية - يتم تتبع المراجعات تلقائيًا
            // عند إجراء تغييرات بعد إنشاء المصنف
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Initial Value");

            // غيّر الخلية لإنشاء مراجعة
            cell.PutValue("Modified Value");

            // الوصول إلى سجلات المراجعة
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange)
                    {
                        // عرض معلومات النوع من المراجعة
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Revision Type: " + cellChange.Type);

                        // إظهار كيفية استخدام خاصية Type
                        if (cellChange.Type == RevisionType.ChangeCells)
                        {
                            Console.WriteLine("\nThis is a cell change revision");
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);
                        }

                        // تحقق من أنواع المراجعة الأخرى الممكنة
                        switch (cellChange.Type)
                        {
                            case RevisionType.ChangeCells:
                                Console.WriteLine("Handling cell value change revision");
                                break;
                            case RevisionType.Format:
                                Console.WriteLine("Handling format change revision");
                                break;
                            default:
                                Console.WriteLine("Handling other type of revision");
                                break;
                        }
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCellChangePropertyTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


