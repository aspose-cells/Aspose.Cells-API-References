---
title: "التعداد SortOnType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.SortOnType. نوع القيمة المرتبة"
type: docs
url: /ar/net/aspose.cells/sortontype/
---
## SortOnType enumeration

نوع القيمة المرتبة.

```csharp
public enum SortOnType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Value | `0` | يتم الفرز حسب قيمة الخلايا. |
| CellColor | `1` | يتم الفرز حسب لون الخلايا. |
| FontColor | `2` | يتم الفرز حسب لون خط الخلايا. |
| Icon | `3` | يتم الفرز حسب الأيقونة الشرطية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SortOnTypeDemo
    {
        public static void SortOnTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(95);
            worksheet.Cells["B4"].PutValue(75);

            // تطبيق الفلتر التلقائي على النطاق
            worksheet.AutoFilter.Range = "A1:B4";

            // الحصول على الفلتر التلقائي
            AutoFilter autoFilter = worksheet.AutoFilter;

            // الحصول على مُرتب البيانات
            DataSorter sorter = autoFilter.Sorter;

            // تعيين المفتاح الأول للفرز حسب القيم في العمود الثاني (النتيجة)
            sorter.AddKey(1, SortOnType.Value, SortOrder.Descending, null);

            // فرز البيانات في النطاق
            sorter.Sort(worksheet.Cells, 1, 0, 3, 1);

            // احفظ المصنف
            workbook.Save("SortOnTypeExample.xlsx");

            // أخرج النتائج
            Console.WriteLine("Data sorted by Score in descending order.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


