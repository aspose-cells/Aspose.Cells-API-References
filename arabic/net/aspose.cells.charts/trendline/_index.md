---
title: "الفئة Trendline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.Trendline. تمثل خط اتجاه في مخطط"
type: docs
url: /ar/net/aspose.cells.charts/trendline/
---
## Trendline class

يمثل خط الاتجاه في المخطط.

```csharp
public class Trendline : Line
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward/) { get; set; } | إرجاع أو تعيين عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد إليها خط الاتجاه إلى الخلف. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. إذا كان نوع المخطط عمودياً، يجب أن يكون عدد الفترات بين 0 و 0.5 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | يحدد طول رأس السهم لبداية الخط. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | يحدد عرض رأس السهم لبداية الخط. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | يحدد رأس سهم لبداية الخط. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | يحدد أغطية النهاية. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | يمثل لون الخط. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | يحدد نوع الخط المركب (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | يحدد نوع الخط المتقطع (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels/) { get; } | يمثل كائن DataLabels للسلسلة المحددة. |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation/) { get; set; } | يمثل ما إذا كانت معادلة خط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كقيمة R-squared). ضبط هذه الخاصية على True يُفعِّل تلقائيًا تسميات البيانات. |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared/) { get; set; } | يمثل ما إذا كانت قيمة R-squared لخط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كالمعادلة). ضبط هذه الخاصية على True يُفعِّل تلقائيًا تسميات البيانات. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | يحدد طول رأس السهم لنهاية الخط. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | يحدد عرض رأس السهم لنهاية الخط. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | يحدد رأس سهم لنهاية الخط. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | الحصول على أو تعيين نوع التنسيق. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [Forward](../../aspose.cells.charts/trendline/forward/) { get; set; } | إرجاع أو تعيين عدد الفترات (أو الوحدات في مخطط مبعثر) التي يمتد إليها خط الاتجاه إلى الأمام. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | يمثل تعبئة متدرجة. (موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [Intercept](../../aspose.cells.charts/trendline/intercept/) { get; set; } | إرجاع أو تعيين النقطة التي يقطع فيها خط الاتجاه محور القيم. |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | يشير إلى ما إذا كان نمط الخط هذا يتم تعيينه تلقائيًا.(موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | يشير إلى ما إذا كان لون الخط يتم تعيينه تلقائيًا.(موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto/) { get; set; } | يعيد ما إذا كان Microsoft Excel يحدد اسم خط الاتجاه تلقائيًا. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | يمثل ما إذا كان الخط مرئيًا.(موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | يحدد أغطية الربط.(موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry/) { get; } | يحصل على مدخل الأسطورة وفقًا لخط الاتجاه هذا |
| [Name](../../aspose.cells.charts/trendline/name/) { get; set; } | يعيد اسم خط الاتجاه. |
| [Order](../../aspose.cells.charts/trendline/order/) { get; set; } | يعيد أو يضبط ترتيب خط الاتجاه (عدد صحيح أكبر من 1) عندما يكون نوع خط الاتجاه متعدد الحدود. يجب أن يكون الترتيب بين 2 و 6. |
| [Period](../../aspose.cells.charts/trendline/period/) { get; set; } | يعيد أو يضبط الفترة لخط الاتجاه المتوسط المتحرك. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | يمثل نمط الخط.(موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | يحصل على ويضبط لون السمة.(موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).(موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [Type](../../aspose.cells.charts/trendline/type/) { get; } | يعيد نوع خط الاتجاه. |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | يحصل على أو يضبط [`WeightType`](../../aspose.cells.drawing/weighttype/) للخط.(موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | يحصل على أو يضبط وزن الخط بوحدة النقاط.(موروث من [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | يحصل على أو يضبط وزن الخط بوحدة البكسل.(موروث من [`Line`](../../aspose.cells.drawing/line/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineDemo
    {
        public static void TrendlineExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            // إضافة ورقة عمل جديدة إلى كائن Excel
            int sheetIndex = workbook.Worksheets.Add();
            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // إضافة قيم عينة إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];
            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B4"
            chart.NSeries.Add("A1:B4", true);
            // تعيين مصدر البيانات لبيانات الفئة في NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // إضافة خط اتجاه خطي
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            // تعيين الاسم المخصص لخط الاتجاه
            trendline.Name = "Linear";
            // عرض المعادلة على المخطط
            trendline.DisplayEquation = true;
            // عرض قيمة R-مربعة على المخطط
            trendline.DisplayRSquared = true;

            // ضبط الخصائص الإضافية
            trendline.IsNameAuto = false;
            trendline.Order = 2;
            trendline.Period = 3;
            trendline.Forward = 1.5;
            trendline.Backward = 0.5;
            trendline.Intercept = 0.0;
            trendline.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
            trendline.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.Dash;
            trendline.CapType = Aspose.Cells.Drawing.LineCapType.Round;
            trendline.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
            trendline.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
            trendline.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
            trendline.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
            trendline.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
            trendline.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
            trendline.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
            trendline.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
            trendline.Color = Color.Red;
            trendline.Transparency = 0.5;
            trendline.Style = Aspose.Cells.Drawing.LineType.DashDot;
            trendline.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
            trendline.WeightPt = 2.0;
            trendline.WeightPx = 3.0;
            trendline.FormattingType = Aspose.Cells.Charts.ChartLineFormattingType.Gradient;
            trendline.IsVisible = true;
            trendline.IsAuto = false;

            // حفظ ملف Excel
            workbook.Save("TrendlineExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Line](../../aspose.cells.drawing/line/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


