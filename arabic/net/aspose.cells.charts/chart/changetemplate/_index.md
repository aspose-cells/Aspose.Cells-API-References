---
title: "Chart.ChangeTemplate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Chart. تغيير نوع المخطط باستخدام قالب مسبق"
type: docs
url: /ar/net/aspose.cells.charts/chart/changetemplate/
---
## Chart.ChangeTemplate method

غيّر نوع المخطط باستخدام قالب مسبق.

```csharp
public void ChangeTemplate(byte[] data)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| بيانات | Byte[] | بيانات ملف قالب المخطط (.crtx). |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodChangeTemplateWithByteDemo
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
            chart.SetChartDataRange("A1:B4", false);

            // احصل على بيانات القالب من ملف مخطط آخر
            byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");

            try
            {
                // استدعِ طريقة ChangeTemplate مع معامل مصفوفة بايت
                chart.ChangeTemplate(templateData);
                
                Console.WriteLine("Chart template changed successfully using byte array parameter");
                
                // اعرض التأثير بحفظ المصنف
                workbook.Save("ChartWithChangedTemplate.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing chart template: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


