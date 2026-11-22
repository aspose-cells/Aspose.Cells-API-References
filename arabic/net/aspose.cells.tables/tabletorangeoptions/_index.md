---
title: "الفئة TableToRangeOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Tables.TableToRangeOptions. تمثل الخيارات عند تحويل الجدول إلى نطاق"
type: docs
url: /ar/net/aspose.cells.tables/tabletorangeoptions/
---
## TableToRangeOptions class

يمثل الخيارات عند تحويل الجدول إلى نطاق.

```csharp
public class TableToRangeOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [TableToRangeOptions](tabletorangeoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [LastRow](../../aspose.cells.tables/tabletorangeoptions/lastrow/) { get; set; } | يحصل على ويضبط فهرس الصف الأخير في الجدول. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableToRangeOptionsDemo
    {
        public static void TableToRangeOptionsExample()
        {
            // إنشاء دفتر عمل جديد
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
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // أضف ListObject (جدول) إلى ورقة العمل
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // ضبط بعض خصائص الجدول
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // إنشاء كائن من TableToRangeOptions
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // تحويل الجدول إلى نطاق باستخدام الخيارات
            table.ConvertToRange(options);

            // احفظ المصنف
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


