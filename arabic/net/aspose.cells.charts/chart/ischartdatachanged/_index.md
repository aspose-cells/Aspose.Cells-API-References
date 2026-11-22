---
title: "Chart.IsChartDataChanged"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Chart. تكتشف ما إذا كان مصدر بيانات المخطط قد تغير"
type: docs
url: /ar/net/aspose.cells.charts/chart/ischartdatachanged/
---
## Chart.IsChartDataChanged method

يكشف ما إذا كان مصدر بيانات المخطط قد تغير.

```csharp
public bool IsChartDataChanged()
```

### قيمة الإرجاع

يرجع true إذا تغير المخطط وإلا يرجع false

### ملاحظات

تكتشف الطريقة التغييرات في مصدر بيانات المخطط قبل تحويل المخطط إلى تنسيق صورة. عند أول استدعاء Chart.toImage، سيتم تسجيل بيانات مصدر المخطط (مثل XValuesParseData، ValuesParseData). قبل استدعاء طريقة Chart.toImage مرة أخرى، استدعِ طريقة IsChartDataChanged للتحقق مما إذا كان المخطط يحتاج إلى إعادة التصيير.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartMethodIsChartDataChangedDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // تحقق مما إذا كانت بيانات المخطط قد تغيرت (يجب أن تكون false في البداية)
                bool isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after creation: {isChanged}");

                // تعديل بيانات المخطط
                worksheet.Cells["B2"].PutValue(15);

                // تحقق مرة أخرى مما إذا كانت بيانات المخطط قد تغيرت
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after modification: {isChanged}");

                // احسب المخطط لتحديثه
                chart.Calculate();

                // تحقق بعد الحساب
                isChanged = chart.IsChartDataChanged();
                Console.WriteLine($"Chart data changed after calculation: {isChanged}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsChartDataChanged method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("ChartMethodIsChartDataChangedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


