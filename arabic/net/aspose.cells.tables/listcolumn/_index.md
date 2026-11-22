---
title: "الفئة ListColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Tables.ListColumn. تمثل عمودًا في جدول"
type: docs
url: /ar/net/aspose.cells.tables/listcolumn/
---
## ListColumn class

يمثل عمودًا في جدول.

```csharp
public class ListColumn
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Formula](../../aspose.cells.tables/listcolumn/formula/) { get; set; } | يحصل على صيغة العمود في القائمة ويضبطها. |
| [IsArrayFormula](../../aspose.cells.tables/listcolumn/isarrayformula/) { get; } | يشير إلى ما إذا كانت الصيغة مصفوفة. |
| [Name](../../aspose.cells.tables/listcolumn/name/) { get; set; } | يحصل على اسم العمود ويضبطه. |
| [Range](../../aspose.cells.tables/listcolumn/range/) { get; } | يحصل على نطاق هذا العمود في القائمة. |
| [TotalsCalculation](../../aspose.cells.tables/listcolumn/totalscalculation/) { get; set; } | يحصل على نوع الحساب في صف الإجماليات للعمود في القائمة ويضبطه. |
| [TotalsRowLabel](../../aspose.cells.tables/listcolumn/totalsrowlabel/) { get; set; } | يحصل على تسميات العرض لصف الإجماليات ويضبطها. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/getcustomcalculatedformula/)(bool, bool) | يحصل على الصيغة لهذا عمود القائمة. |
| [GetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/getcustomtotalsrowformula/)(bool, bool) | يحصل على صيغة صف الإجماليات لهذا عمود القائمة. |
| [GetDataStyle](../../aspose.cells.tables/listcolumn/getdatastyle/)() | يحصل على نمط البيانات في هذا العمود من الجدول. |
| [SetCustomCalculatedFormula](../../aspose.cells.tables/listcolumn/setcustomcalculatedformula/)(string, bool, bool) | يضبط الصيغة لهذا عمود القائمة. |
| [SetCustomTotalsRowFormula](../../aspose.cells.tables/listcolumn/setcustomtotalsrowformula/)(string, bool, bool) | يحصل على صيغة صف الإجماليات لهذا عمود القائمة. |
| [SetDataStyle](../../aspose.cells.tables/listcolumn/setdatastyle/)(Style) | يضبط نمط البيانات في هذا العمود من الجدول. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnDemo
    {
        public static void ListColumnExample()
        {
            // إنشاء مصنف جديد والوصول إلى ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

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

            // أضف ListObject (جدول) إلى ورقة العمل
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];
            table.ShowTotals = true;

            // الوصول إلى ListColumn وتعيين خصائصه
            ListColumn listColumn = table.ListColumns[4];
            listColumn.TotalsCalculation = TotalsCalculation.Sum;
            listColumn.Formula = "=[A]";
            listColumn.Name = "CustomColumn";
            listColumn.TotalsRowLabel = "Total";

            // احفظ المصنف
            workbook.Save("ListColumnExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


