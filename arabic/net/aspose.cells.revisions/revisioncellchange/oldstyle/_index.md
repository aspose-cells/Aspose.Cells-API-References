---
title: "RevisionCellChange.OldStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RevisionCellChange. يحصل على النمط القديم للخلية"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellchange/oldstyle/
---
## RevisionCellChange.OldStyle property

يحصل على النمط القديم للخلية.

```csharp
public Style OldStyle { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyOldStyleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد مع تتبع المراجعات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين النمط الأولي للخلية A1
            Cell cell = worksheet.Cells["A1"];
            Style initialStyle = workbook.CreateStyle();
            initialStyle.Font.Name = "Arial";
            initialStyle.Font.Size = 10;
            initialStyle.Font.Color = System.Drawing.Color.Black;
            cell.SetStyle(initialStyle);
            cell.PutValue("Initial Value");

            // تغيير نمط الخلية لإنشاء مراجعة
            Style newStyle = workbook.CreateStyle();
            newStyle.Font.Name = "Times New Roman";
            newStyle.Font.Size = 12;
            newStyle.Font.Color = System.Drawing.Color.Red;
            newStyle.Font.IsBold = true;
            cell.SetStyle(newStyle);
            cell.PutValue("Modified Value");

            // الوصول إلى سجلات المراجعة
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            foreach (RevisionLog log in revisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    if (revision is RevisionCellChange cellChange && cellChange.CellName == "A1")
                    {
                        // عرض معلومات تغيير النمط
                        Console.WriteLine("Cell Name: " + cellChange.CellName);
                        Console.WriteLine("Old Style Font: " + cellChange.OldStyle.Font.Name);
                        Console.WriteLine("Old Style Size: " + cellChange.OldStyle.Font.Size);
                        Console.WriteLine("Old Style Color: " + cellChange.OldStyle.Font.Color);
                        Console.WriteLine("New Style Font: " + cellChange.NewStyle.Font.Name);
                        Console.WriteLine("New Style Size: " + cellChange.NewStyle.Font.Size);
                        Console.WriteLine("New Style Color: " + cellChange.NewStyle.Font.Color);

                        // إظهار كيفية استخدام الخاصية OldStyle
                        if (cellChange.OldStyle.Font.Name == "Arial")
                        {
                            Console.WriteLine("\nThe cell originally had Arial font");
                        }
                    }
                }
            }

            // احفظ المصنف مع التعديلات
            workbook.Save("RevisionCellChangePropertyOldStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../../aspose.cells/style/)
* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


