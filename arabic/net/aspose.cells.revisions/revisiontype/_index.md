---
title: "تعداد RevisionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Revisions.RevisionType تعداد. يمثل نوع المراجعة"
type: docs
url: /ar/net/aspose.cells.revisions/revisiontype/
---
## RevisionType enumeration

يمثل نوع المراجعة.

```csharp
public enum RevisionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| CustomView | `0` | عرض مخصص. |
| DefinedName | `1` | اسم معرف. |
| ChangeCells | `2` | تغيير الخلايا. |
| AutoFormat | `3` | تنسيق تلقائي. |
| MergeConflict | `4` | تعارض دمج. |
| Comment | `5` | تعليق. |
| Format | `6` | تنسيق. |
| InsertSheet | `7` | إدراج ورقة عمل. |
| MoveCells | `8` | نقل الخلايا. |
| Undo | `9` | تراجع. |
| QueryTable | `10` | استعلام الجدول. |
| InsertDelete | `11` | الإدراج أو الحذف. |
| RenameSheet | `12` | إعادة تسمية ورقة العمل. |
| Unknown | `13` | غير معروف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // عرض استخدام قيم مختلفة لتعداد RevisionType
                RevisionType customViewType = RevisionType.CustomView;
                RevisionType changeCellsType = RevisionType.ChangeCells;
                RevisionType insertSheetType = RevisionType.InsertSheet;

                // عرض قيم enum والقيم الصحيحة الأساسية لها
                Console.WriteLine("CustomView type: " + customViewType + " (Value: " + (int)customViewType + ")");
                Console.WriteLine("ChangeCells type: " + changeCellsType + " (Value: " + (int)changeCellsType + ")");
                Console.WriteLine("InsertSheet type: " + insertSheetType + " (Value: " + (int)insertSheetType + ")");

                // عرض فحص أنواع المراجعات
                if (workbook.HasRevisions)
                {
                    Console.WriteLine("Workbook contains revisions");
                }
                else
                {
                    Console.WriteLine("Workbook has no revisions");
                }

                // احفظ المصنف
                workbook.Save("RevisionTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


