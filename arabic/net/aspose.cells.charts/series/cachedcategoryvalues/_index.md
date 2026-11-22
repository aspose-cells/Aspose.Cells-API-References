---
title: "Series.CachedCategoryValues"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. يحصل على قيم الفئات المخزنة مؤقتًا للسلسلة"
type: docs
url: /ar/net/aspose.cells.charts/series/cachedcategoryvalues/
---
## Series.CachedCategoryValues property

يحصل على قيم الفئات المخزنة مؤقتًا للسلسلة

```csharp
[Obsolete("internal use only")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList CachedCategoryValues { get; }
```

### ملاحظات

ملاحظة: هذه الخاصية مخصصة للاستخدام الداخلي حاليًا فقط. سيتم تغييرها أو إزالتها في الإصدار التالي.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Collections;

    public class SeriesPropertyCachedCategoryValuesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // الوصول إلى السلسلة الأولى
                Series series = chart.NSeries[0];

                // اعرض قيم الفئات المخزنة مؤقتًا
                ArrayList cachedCategoryValues = series.CachedCategoryValues;
                Console.WriteLine("CachedCategoryValues count: " + cachedCategoryValues.Count);

                // اعرض كل قيمة فئة مخزنة مؤقتًا
                for (int i = 0; i < cachedCategoryValues.Count; i++)
                {
                    Console.WriteLine("Cached Category Value " + (i + 1) + ": " + cachedCategoryValues[i]);
                }

                // احفظ المصنف
                workbook.Save("CachedCategoryValuesDemo.xlsx");
                Console.WriteLine("CachedCategoryValues demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


