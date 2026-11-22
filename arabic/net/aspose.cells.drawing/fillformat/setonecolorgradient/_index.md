---
title: "FillFormat.SetOneColorGradient"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FillFormat. تعيين الملء المحدد إلى تدرج لون واحد. ينطبق فقط على Excel 2007"
type: docs
url: /ar/net/aspose.cells.drawing/fillformat/setonecolorgradient/
---
## FillFormat.SetOneColorGradient method

يضبط الملء المحدد إلى تدرج بلون واحد. ينطبق فقط على Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| اللون | اللون | لون تدرج واحد. |
| درجة | Double | درجة التدرج. يمكن أن تكون قيمة من 0.0 (غامق) إلى 1.0 (فاتح). |
| النمط | GradientStyleType | نمط تظليل التدرج. |
| variant | Int32 | متغير التدرج. يمكن أن يكون قيمة من 1 إلى 4، المقابل لأحد المتغيرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان style هو GradientStyle.FromCenter، فإن معامل Variant لا يمكن أن يكون إلا 1 أو 2. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تطبيق تعبئة التدرج على السلسلة الأولى
            Series series = chart.NSeries[0];
            series.IsColorVaried = false;
            
            // عرض مثال لـ SetOneColorGradient مع معلمات محددة
            series.Area.FillFormat.SetOneColorGradient(
                Color.FromArgb(0, 236, 102, 102), // Color
                0.9,                              // Transparency
                Aspose.Cells.Drawing.GradientStyleType.DiagonalDown,    // Gradient style
                2);                                // Variant

            // احفظ المصنف
            workbook.Save("FillFormat_SetOneColorGradient_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


