---
title: "الفئة TickLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.TickLabels. تمثّل تسميات علامات الفواصل المرتبطة بعلامات الفواصل على محور المخطط"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/
---
## TickLabels class

يمثل تسميات علامات التحديد المرتبطة بعلامات التحديد على محور المخطط.

```csharp
public class TickLabels
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AlignmentType](../../aspose.cells.charts/ticklabels/alignmenttype/) { get; set; } | يحصل أو يعيّن محاذاة النص لتسميات علامات الفواصل على المحور. |
| [AutoScaleFont](../../aspose.cells.charts/ticklabels/autoscalefont/) { get; set; } | صحيح إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True. |
| [BackgroundMode](../../aspose.cells.charts/ticklabels/backgroundmode/) { get; set; } | يحصل ويضبط وضع عرض الخلفية. |
| [DirectionType](../../aspose.cells.charts/ticklabels/directiontype/) { get; set; } | يحصل على اتجاه النص ويضبطه. |
| [DisplayNumberFormat](../../aspose.cells.charts/ticklabels/displaynumberformat/) { get; } | يحصل أو يعيّن تنسيق الأرقام المعروض لتسميات علامات الفواصل. |
| [Font](../../aspose.cells.charts/ticklabels/font/) { get; } | يرجع كائن [`Font`](./font/) يمثل خط الكائن TickLabels المحدد. |
| [IsAutomaticRotation](../../aspose.cells.charts/ticklabels/isautomaticrotation/) { get; set; } | يشير إلى ما إذا كان زاوية الدوران تلقائية |
| [Number](../../aspose.cells.charts/ticklabels/number/) { get; set; } | تمثّل رقم التنسيق لكائن TickLabels. |
| [NumberFormat](../../aspose.cells.charts/ticklabels/numberformat/) { get; set; } | تمثّل سلسلة التنسيق لكائن TickLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/ticklabels/numberformatlinked/) { get; set; } | صحيح إذا كان تنسيق الرقم مرتبطًا بالخلايا (بحيث يتغير تنسيق الرقم في التسميات عندما يتغير في الخلايا). |
| [Offset](../../aspose.cells.charts/ticklabels/offset/) { get; set; } | يحصل أو يعيّن مسافة التسميات من محور الفئة. ينطبق هذا فقط على محور الفئة (x). |
| [ReadingOrder](../../aspose.cells.charts/ticklabels/readingorder/) { get; set; } | يمثل ترتيب قراءة النص. |
| [RotationAngle](../../aspose.cells.charts/ticklabels/rotationangle/) { get; set; } | يمثل زاوية دوران النص باتجاه عقارب الساعة. |
| [TextDirection](../../aspose.cells.charts/ticklabels/textdirection/) { get; set; } | (**Obsolete.**) يمثل ترتيب قراءة النص. |
| [TickLabelItems](../../aspose.cells.charts/ticklabels/ticklabelitems/) { get; } | يحصل على تسميات العلامات المعروضة للمحور. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelsDemo
    {
        public static void TickLabelsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // أضف NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية \"A1\" إلى \"B3\"
            chart.NSeries.Add("A1:B3", true);

            // الوصول إلى محور القيم
            Axis valueAxis = chart.ValueAxis;

            // الوصول إلى تسميات العلامات لمحور القيم
            TickLabels tickLabels = valueAxis.TickLabels;

            // تعيين خصائص تسميات العلامات
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = "0.00";
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // احفظ المصنف
            workbook.Save("TickLabelsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


