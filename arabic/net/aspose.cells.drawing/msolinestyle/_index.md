---
title: "تعداد MsoLineStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.MsoLineStyle. يمثل نمط خطوط الرسم"
type: docs
url: /ar/net/aspose.cells.drawing/msolinestyle/
---
## MsoLineStyle enumeration

يمثل نمط خطوط الرسم.

```csharp
public enum MsoLineStyle
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Single | `0` | خط واحد (بعرض lineWidth) |
| ThickBetweenThin | `1` | ثلاثة خطوط، رفيع، سميك، رفيع |
| ThinThick | `2` | خطين مزدوجين، أحدهما رفيع، والآخر سميك |
| ThickThin | `3` | خطين مزدوجين، أحدهما سميك، والآخر رفيع |
| ThinThin | `4` | خطين مزدوجين بعرض متساوٍ |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineStyleDemo
    {
        public static void MsoLineStyleExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى محور الفئة الأساسي
            Axis categoryAxis = chart.CategoryAxis;

            // تعيين نمط الخط لمحور الفئة الأساسي
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // إخراج نمط الخط
            Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
            Console.WriteLine("Axis Line Color: " + axisLine.Color);
            Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);

            // احفظ المصنف
            workbook.Save("MsoLineStyleExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


