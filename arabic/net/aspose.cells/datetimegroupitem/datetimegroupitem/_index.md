---
title: "DateTimeGroupItem.DateTimeGroupItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ DateTimeGroupItem."
type: docs
url: /ar/net/aspose.cells/datetimegroupitem/datetimegroupitem/
---
## DateTimeGroupItem constructor

```csharp
public DateTimeGroupItem(DateTimeGroupingType type, int year, int month, int day, int hour, 
    int minute, int second)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | DateTimeGroupingType |  |
| سنة | Int32 |  |
| شهر | Int32 |  |
| يوم | Int32 |  |
| ساعة | Int32 |  |
| دقيقة | Int32 |  |
| ثانية | Int32 |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DateTimeGroupItemMethodCtorWithDateTimeGroupingTypeInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد والوصول إلى الورقة الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات تاريخ ووقت نموذجية إلى العمود A
            worksheet.Cells["A1"].PutValue("Order Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 3, 15, 9, 30, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 4, 20, 14, 15, 45));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 25, 10, 0, 0));
            worksheet.Cells["A5"].PutValue(new DateTime(2024, 3, 1, 8, 45, 30));

            // تطبيق الفلتر التلقائي على عمود التاريخ
            worksheet.AutoFilter.Range = "A1:A5";

            try
            {
                // إنشاء DateTimeGroupItem لتجميع مارس 2023
                DateTimeGroupItem groupItem = new DateTimeGroupItem(
                    DateTimeGroupingType.Month, // Group by Month
                    2023,   // Year
                    3,      // Month (March)
                    1,      // Day (ignored in Month grouping)
                    0,      // Hour
                    0,      // Minute
                    0       // Second
                );

                // تكوين الفلتر لإظهار تواريخ مارس 2023
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
                filterColumn.FilterType = FilterType.MultipleFilters;
                filterColumn.Filter = groupItem;

                // تحديث الفلتر لتطبيق التغييرات
                worksheet.AutoFilter.Refresh();

                Console.WriteLine("DateTimeGroupItem created and filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying date filter: {ex.Message}");
            }

            // حفظ المصنف المفلتر
            workbook.Save("DateTimeGroupItemConstructorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [DateTimeGroupingType](../../datetimegroupingtype/)
* class [DateTimeGroupItem](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


