---
title: "تعداد MergedCellsShrinkType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.MergedCellsShrinkType. يمثل الاستراتيجية لتقليص الخلايا المدمجة للعمليات مثل حذف الصفوف/الأعمدة الفارغة."
type: docs
url: /ar/net/aspose.cells/mergedcellsshrinktype/
---
## MergedCellsShrinkType enumeration

يمثل الاستراتيجية لتقليص الخلايا المدمجة للعمليات مثل حذف الصفوف/الأعمدة الفارغة.

```csharp
public enum MergedCellsShrinkType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يترك الخلايا المدمجة كما هي دون أي تعديل. |
| ShrinkToFit | `1` | يقوم بتقليص المنطقة المدمجة إذا لزم الأمر، بإزالة الصفوف من الأسفل أو الأعمدة من اليمين، مع ضمان بقاء جميع المحتويات مرئية. |
| KeepHeaderOnly | `2` | يحتفظ فقط بصفوف/أعمدة العنوان للمنطقة المدمجة عندما لا تكون الخلية العلوية اليسرى للمنطقة المدمجة فارغة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassMergedCellsShrinkTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            Cells cells = ws.Cells;

            // تهيئة بيانات تجريبية مع خلايا مدمجة
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            Console.WriteLine("Original worksheet:");
            PrintCellValues(cells);

            // الخيار 1: KeepHeaderOnly
            DeleteBlankOptions opts1 = new DeleteBlankOptions();
            opts1.MergedCellsShrinkType = MergedCellsShrinkType.KeepHeaderOnly;
            cells.DeleteBlankColumns(opts1);
            Console.WriteLine("\nAfter DeleteBlankColumns with KeepHeaderOnly:");
            PrintCellValues(cells);

            // إعادة تعيين ورقة العمل
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // الخيار 2: لا شيء
            DeleteBlankOptions opts2 = new DeleteBlankOptions();
            opts2.MergedCellsShrinkType = MergedCellsShrinkType.None;
            cells.DeleteBlankColumns(opts2);
            Console.WriteLine("\nAfter DeleteBlankColumns with None:");
            PrintCellValues(cells);

            // إعادة تعيين ورقة العمل
            cells.ClearContents(0, 0, cells.MaxDataRow, cells.MaxDataColumn);
            cells.Merge(0, 0, 1, 2);
            cells[0, 0].PutValue("Merged Header");
            cells[1, 2].PutValue("Data 1");
            cells[2, 2].PutValue("Data 2");

            // الخيار 3: ShrinkToFit
            DeleteBlankOptions opts3 = new DeleteBlankOptions();
            opts3.MergedCellsShrinkType = MergedCellsShrinkType.ShrinkToFit;
            cells.DeleteBlankColumns(opts3);
            Console.WriteLine("\nAfter DeleteBlankColumns with ShrinkToFit:");
            PrintCellValues(cells);
        }

        private static void PrintCellValues(Cells cells)
        {
            for (int row = 0; row < 3; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Console.Write($"({row},{col}): {cells[row, col].Value ?? "empty"} | ");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


