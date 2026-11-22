---
title: "Axis.AxisLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المحور. تحصل على تسميات المحور بعد استدعاء طريقة Chart.Calculate"
type: docs
url: /ar/net/aspose.cells.charts/axis/axislabels/
---
## Axis.AxisLabels property

يحصل على تسميات المحور بعد استدعاء طريقة Chart.Calculate().

```csharp
[Obsolete("Use Axis.GetAxisTexts method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList AxisLabels { get; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام طريقة Axis.GetAxisTexts. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ نوفمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyAxisLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
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

            try
            {
                // إضافة مخطط إلى ورقة العمل
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // تعيين نطاق بيانات المخطط
                chart.NSeries.Add("B2:B4", true);
                chart.NSeries.CategoryData = "A2:A4";

                // احسب المخطط لتوليد تسميات المحور
                chart.Calculate();

                // الوصول إلى محور الفئة والحصول على تسميات المحور
                Axis categoryAxis = chart.CategoryAxis;
                var axisLabels = categoryAxis.AxisLabels;

                // عرض تسميات المحور
                Console.WriteLine("Axis Labels:");
                if (axisLabels != null)
                {
                    foreach (var label in axisLabels)
                    {
                        Console.WriteLine(label);
                    }
                }
                else
                {
                    Console.WriteLine("No axis labels available.");
                }

                // احفظ المصنف
                workbook.Save("AxisPropertyAxisLabelsDemo.xlsx");
                Console.WriteLine("AxisLabels demonstration completed successfully.");
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

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


