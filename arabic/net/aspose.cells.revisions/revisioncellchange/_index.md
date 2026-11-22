---
title: "الفئة RevisionCellChange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.RevisionCellChange الفئة. تمثل المراجعة التي تغير الخلايا"
type: docs
url: /ar/net/aspose.cells.revisions/revisioncellchange/
---
## RevisionCellChange class

يمثل المراجعة التي تغير الخلايا.

```csharp
public class RevisionCellChange : Revision
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CellName](../../aspose.cells.revisions/revisioncellchange/cellname/) { get; } | يحصل على اسم الخلية. |
| [Column](../../aspose.cells.revisions/revisioncellchange/column/) { get; } | يحصل على فهرس العمود للخلية. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | يحصل على رقم هذه المراجعة.(موروث من [`Revision`](../revision/).) |
| [IsNewFormatted](../../aspose.cells.revisions/revisioncellchange/isnewformatted/) { get; } | يشير إلى ما إذا كانت هذه الخلية مُنسقة حديثًا. |
| [IsOldFormatted](../../aspose.cells.revisions/revisioncellchange/isoldformatted/) { get; } | يشير إلى ما إذا كانت هذه الخلية مُنسقة قديمًا. |
| [NewFormula](../../aspose.cells.revisions/revisioncellchange/newformula/) { get; } | يحصل على الصيغة القديمة. |
| [NewStyle](../../aspose.cells.revisions/revisioncellchange/newstyle/) { get; } | يحصل على النمط الجديد للخلية. |
| [NewValue](../../aspose.cells.revisions/revisioncellchange/newvalue/) { get; } | يحصل على القيمة الجديدة للخلية. |
| [OldFormula](../../aspose.cells.revisions/revisioncellchange/oldformula/) { get; } | يحصل على الصيغة القديمة. |
| [OldStyle](../../aspose.cells.revisions/revisioncellchange/oldstyle/) { get; } | يحصل على النمط القديم للخلية. |
| [OldValue](../../aspose.cells.revisions/revisioncellchange/oldvalue/) { get; } | يحصل على القيمة القديمة للخلية. |
| [Row](../../aspose.cells.revisions/revisioncellchange/row/) { get; } | يحصل على فهرس الصف للخلية. |
| override [Type](../../aspose.cells.revisions/revisioncellchange/type/) { get; } | يمثل نوع المراجعة. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | يحصل على ورقة العمل. (موروث من [`Revision`](../revision/).) |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionsClassRevisionCellChangeDemo
    {
        public static void Run()
        {
            // أنشئ دليل الإخراج إذا لم يكن موجودًا
            string outputDir = "output/";
            System.IO.Directory.CreateDirectory(outputDir);
            
            string filePath = outputDir + "RevisionsClassRevisionCellChangeDemo_out.xlsx";

            // أنشئ دفتر العمل الأولي وفعّل المشاركة
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Save(filePath, SaveFormat.Xlsx);

            // أعد فتح دفتر العمل لإجراء تغييرات متتبعة
            Workbook workbook2 = new Workbook(filePath);
            Worksheet sheet = workbook2.Worksheets[0];
            
            // المراجعة الأولى: تعيين القيم الأولية
            sheet.Cells["A1"].PutValue("Initial Value");
            sheet.Cells["B2"].PutValue(100);
            workbook2.Save(filePath, SaveFormat.Xlsx);
            
            // المراجعة الثانية: تعديل القيم
            sheet.Cells["A1"].PutValue("Updated Value");
            sheet.Cells["B2"].PutValue(200);
            workbook2.Save(filePath, SaveFormat.Xlsx);

            // حمّل دفتر العمل للوصول إلى سجلات المراجعات
            Workbook workbook3 = new Workbook(filePath);
            
            // معالجة جميع سجلات المراجعات
            foreach (RevisionLog log in workbook3.Worksheets.RevisionLogs)
            {
                foreach (Revision rev in log.Revisions)
                {
                    if (rev.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange rcc = (RevisionCellChange)rev;
                        Console.WriteLine($"Revision Type: {rev.Type}");
                        Console.WriteLine($"Cell: {rcc.CellName} (Row: {rcc.Row}, Column: {rcc.Column})");
                        Console.WriteLine($"Old Value: {rcc.OldValue ?? "null"}");
                        Console.WriteLine($"New Value: {rcc.NewValue ?? "null"}");
                        Console.WriteLine("------------------------------------");
                    }
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


