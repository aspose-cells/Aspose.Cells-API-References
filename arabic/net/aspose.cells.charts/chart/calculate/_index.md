---
title: "Chart.Calculate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Chart. تحسب المواضع المخصصة لمنطقة الرسم والمحاور إذا تم تعيين مواضعها تلقائيًا"
type: docs
url: /ar/net/aspose.cells.charts/chart/calculate/
---
## Calculate() {#calculate}

يحسب المواضع المخصصة لمنطقة المخطط والمحاور إذا تم تعيين مواضعها تلقائيًا.

```csharp
public void Calculate()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احسب المخطط قبل الحفظ
            chart.Calculate();

            // احفظ المصنف مع المخطط
            workbook.Save("ChartCalculateDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Calculate(ChartCalculateOptions) {#calculate_1}

يحسب الموضع المخصص لمنطقة المخطط والمحاور إذا تم تعيين موضعها تلقائيًا، باستخدام خيارات حساب المخطط.

```csharp
public void Calculate(ChartCalculateOptions calculateOptions)
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateWithChartCalculateOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تمكين تسميات البيانات
            chart.NSeries[0].DataLabels.ShowValue = true;

            // إنشاء خيارات الحساب وتعيينها لتحديث جميع النقاط
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;

            // احسب المخطط باستخدام الخيارات
            chart.Calculate(calculateOptions);

            // أخرج نصوص تسميات البيانات
            ChartPointCollection points = chart.NSeries[0].Points;
            Console.WriteLine("DataLabel Text for Point 0: " + points[0].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 1: " + points[1].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 2: " + points[2].DataLabels.Text);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartCalculateOptions](../../chartcalculateoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


