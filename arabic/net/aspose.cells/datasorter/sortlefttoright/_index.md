---
title: "DataSorter.SortLeftToRight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorter. True يعني أن اتجاه الفرز من اليسار إلى اليمين. False يعني أن اتجاه الفرز من الأعلى إلى الأسفل. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/datasorter/sortlefttoright/
---
## DataSorter.SortLeftToRight property

صحيح يعني أن اتجاه الفرز من اليسار إلى اليمين. خطأ يعني أن اتجاه الفرز من الأعلى إلى الأسفل. القيمة الافتراضية هي خطأ.

```csharp
public bool SortLeftToRight { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortLeftToRightDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة (سيتم التعامل مع الأعمدة كصفوف عندما SortLeftToRight=true)
            worksheet.Cells["A1"].PutValue(3);
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("C");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");

            // إنشاء مُرتّب بيانات وتعيينه للفرز من اليسار إلى اليمين
            DataSorter sorter = workbook.DataSorter;
            sorter.SortLeftToRight = true;

            // تعيين مفتاح الفرز (يصبح فهرس العمود فهرس الصف عند الفرز من اليسار إلى اليمين)
            sorter.Key1 = 0; // Sort by first "row" (originally column A)

            // تحديد منطقة الفرز (تتحول الصفوف إلى أعمدة عند الفرز من اليسار إلى اليمين)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 2;
            area.StartColumn = 0;
            area.EndColumn = 1;

            // تنفيذ الفرز
            sorter.Sort(worksheet.Cells, area);

            // حفظ النتيجة
            workbook.Save("SortedLeftToRight.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


