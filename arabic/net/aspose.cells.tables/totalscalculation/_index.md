---
title: "التعداد TotalsCalculation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Tables.TotalsCalculation. يحدد نوع الحساب في صف الإجماليات لعمود القائمة"
type: docs
url: /ar/net/aspose.cells.tables/totalscalculation/
---
## TotalsCalculation enumeration

يحدد نوع الحساب في صف الإجماليات لعمود القائمة.

```csharp
public enum TotalsCalculation
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Sum | `6` | يمثل حساب إجماليات الجمع. |
| Count | `2` | يمثل حساب إجماليات العد. |
| Average | `1` | يمثل حساب إجماليات المتوسط. |
| Max | `4` | يمثل حساب إجماليات الحد الأقصى. |
| Min | `5` | يمثل حساب إجماليات الحد الأدنى. |
| Var | `8` | يمثل حساب إجماليات التباين. |
| CountNums | `3` | يمثل حساب إجماليات عدد الأرقام. |
| StdDev | `7` | يمثل حساب إجماليات الانحراف المعياري. |
| None | `0` | يمثل عدم حساب إجماليات. |
| Custom | `9` | يمثل حسابًا مخصصًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TotalsCalculationDemo
    {
        public static void TotalsCalculationExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // املأ ورقة العمل ببعض البيانات
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // إضافة جدول إلى ورقة العمل
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // إظهار صف الإجماليات
            table.ShowTotals = true;

            // الوصول إلى العمود الخامس في الجدول
            ListColumn listColumn = table.ListColumns[4];

            // تعيين الخاصية TotalsCalculation إلى Sum
            listColumn.TotalsCalculation = TotalsCalculation.Sum;

            // اختياريًا، تعيين صيغة للعمود
            listColumn.Formula = "=[A]";

            // احفظ المصنف
            workbook.Save("TotalsCalculationExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


