---
title: "ChartCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartCollection. يحصل على عنصر Chart عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.charts/chartcollection/item/
---
## ChartCollection indexer (1 of 2)

يحصل على عنصر [`Chart`](../../chart/) عند الفهرس المحدد.

```csharp
public Chart this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            
            // الوصول إلى المخطط باستخدام خاصية Item
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط والعنوان
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Title.Text = "Sample Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Chart created successfully with Item property access.");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## ChartCollection indexer (2 of 2)

يحصل على المخطط بالاسم.

```csharp
public Chart this[string name] { get; }
```

| معامل | الوصف |
| --- | --- |
| name | اسم المخطط. |

### قيمة الإرجاع

المخطط.

### ملاحظات

اسم المخطط الافتراضي هو null. لذلك يجب عليك تعيين اسم المخطط صراحةً.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // إضافة مخطط إلى ورقة العمل
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);

                // الوصول إلى المخطط باستخدام خاصية Item (المؤشر)
                Chart chart = worksheet.Charts[chartIndex];

                // عرض المعلومات حول المخطط
                Console.WriteLine("Chart type: " + chart.Type);
                Console.WriteLine("Chart name: " + chart.Name);

                // احفظ المصنف
                workbook.Save("ChartCollectionItemDemo.xlsx");

                Console.WriteLine("Chart created and accessed successfully using Item property.");
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

* class [Chart](../../chart/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


