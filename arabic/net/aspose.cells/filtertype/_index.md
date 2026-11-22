---
title: "تعداد FilterType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.FilterType. نوع الفلتر"
type: docs
url: /ar/net/aspose.cells/filtertype/
---
## FilterType enumeration

نوع الفلتر.

```csharp
public enum FilterType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| ColorFilter | `0` | تصفية حسب لون تعبئة الخلية. |
| CustomFilters | `1` | نوع الفلتر المخصص. |
| DynamicFilter | `2` | نوع الفلتر الديناميكي. |
| MultipleFilters | `3` | عند اختيار قيم متعددة للتصفية، أو عند اختيار مجموعة من قيم التاريخ للتصفية، يقوم هذا العنصر بتجميع تلك المعايير معًا. |
| IconFilter | `4` | تصفية حسب أيقونة التنسيق الشرطي. |
| Top10 | `5` | تصفية أعلى 10. |
| None | `6` | بدون تصفية. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFilterTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Color");
            worksheet.Cells["A2"].PutValue("Red");
            worksheet.Cells["A3"].PutValue("Green");
            worksheet.Cells["A4"].PutValue("Blue");
            
            // إنشاء مرشح تلقائي
            worksheet.AutoFilter.Range = "A1:A4";
            AutoFilter filter = worksheet.AutoFilter;
            
            // إنشاء تصفية لون
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            
            // إضافة تصفية لون إلى العمود
            filter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            filter.Refresh();
            
            // التحقق من نوع الفلتر
            FilterColumn filterColumn = filter.FilterColumns[0];
            Console.WriteLine("Filter Type: " + filterColumn.FilterType);
            
            // التحقق من خصائص تصفية اللون
            if (filterColumn.FilterType == FilterType.ColorFilter)
            {
                ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
                Console.WriteLine("Filter by fill color: " + colorFilter.FilterByFillColor);
                Console.WriteLine("Filter color: " + colorFilter.GetColor(workbook.Worksheets));
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


