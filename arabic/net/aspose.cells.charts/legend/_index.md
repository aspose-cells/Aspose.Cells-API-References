---
title: "فئة Legend"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Charts.Legend. تغلف الكائن الذي يمثل وسيلة إيضاح المخطط"
type: docs
url: /ar/net/aspose.cells.charts/legend/
---
## Legend class

يحتوي على الكائن الذي يمثل مفتاح المخطط.

```csharp
public class Legend : ChartTextFrame
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | يحصل على [`area`](../chartframe/area/).(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | صحيح إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True.(موروث من [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) يحصل ويضبط وضع عرض الخلفية. هذه الخاصية صالحة فقط في Excel 2003 أو الإصدارات الأقدم.(موروث من [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode/) { get; set; } | (**Obsolete.**) يحصل ويضبط وضع عرض الخلفية. هذه الخاصية صالحة فقط في Excel 2003 أو الإصدارات الأقدم.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [Border](../../aspose.cells.charts/chartframe/border/) { get; } | يحصل على [`border`](../../aspose.cells.drawing/line/).(موروث من [`ChartFrame`](../chartframe/).) |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) يمثل ارتفاع الموضع الافتراضي بوحدات 1/4000 من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | يمثل ارتفاع الموضع الافتراضي بوحدات جزء من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) يمثل عرض الموضع الافتراضي بوحدات 1/4000 من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | يمثل عرض الموضع الافتراضي بوحدات جزء من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) يمثل إحداثي x للموضع الافتراضي بوحدات 1/4000 من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | يمثل إحداثي x للموضع الافتراضي بوحدات جزء من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) يمثل إحداثي y للموضع الافتراضي بوحدات 1/4000 من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | يمثل إحداثي y للموضع الافتراضي بوحدات جزء من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype/) { get; set; } | الحصول على وتعيين اتجاه النص.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| virtual [Font](../../aspose.cells.charts/chartframe/font/) { get; } | الحصول على كائن [`Font`](../chartframe/font/) لإطار ChartFrame المحدد.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) الحصول على أو تعيين ارتفاع الإطار بوحدات 1/4000 من مساحة المخطط.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | الحصول على أو تعيين ارتفاع الإطار بوحدات البكسل.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | الحصول على أو تعيين ارتفاع الإطار بوحدات نسبة مساحة المخطط.(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | يشير إلى ما إذا كان نص المخطط يدور تلقائيًا.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | يشير إلى ما إذا كان إطار المخطط يتم تحجيمه تلقائيًا.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext/) { get; set; } | يشير إلى أن النص يتم إنشاؤه تلقائيًا.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | يشير إلى ما إذا تم تعيين الموضع الافتراضي (DefaultX، DefaultY، DefaultWidth و DefaultHeight).(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | يشير إلى ما إذا تم حذف تسمية البيانات هذه.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | يشير إلى ما إذا كان حجم مساحة الرسم البياني يشمل علامات الفواصل وعناوين المحاور. القيمة False تحدد أن الحجم سيحدد حجم مساحة الرسم البياني، وعلامات الفواصل، وعناوين المحاور.(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay/) { get; set; } | يحصل أو يضبط ما إذا كان يتم عرض وسيلة الإيضاح دون تداخلها مع المخطط. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | الحصول على أو تعيين ما إذا كان يجب أن يتناسب الشكل تلقائيًا لاحتواء النص الموصوف بداخله بالكامل. التناسب التلقائي هو عندما يتم تحجيم النص داخل الشكل لاحتواء جميع النص داخل الشكل.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان النص مكسورًا.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries/) { get; } | يحصل على مجموعة من جميع كائنات LegendEntry في وسيلة إيضاح المخطط المحددة. لا يدعم ضبط إدخالات وسيلة الإيضاح للمخطط السطحي. لذلك سيعيد null إذا كان نوع المخطط هو نوع المخطط السطحي. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels/) { get; } | (**Obsolete.**) يحصل على تسميات إدخالات وسيلة الإيضاح بعد استدعاء طريقة Chart.Calculate(). |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | الحصول على وتعيين إشارة إلى ورقة العمل.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [Position](../../aspose.cells.charts/legend/position/) { get; set; } | يحصل أو يضبط نوع موضع وسيلة الإيضاح. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | يمثل ترتيب قراءة النص.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | يمثل زاوية دوران النص.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | صحيح إذا كان للإطار ظل.(مستمد من [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | الحصول على كائن [`ShapeProperties`](../chartframe/shapeproperties/).(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [Text](../../aspose.cells.charts/charttextframe/text/) { get; set; } | يحصل على نص عنوان الإطار.(موروث من [`ChartTextFrame`](../charttextframe/).) |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) يمثل ترتيب قراءة النص.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) الحصول على كائن [`Font`](../chartframe/font/) لإطار ChartFrame المحدد.(مستمد من [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | الحصول على وتعيين محاذاة النص الأفقية.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | الحصول على وتعيين خيارات النص.(مستمد من [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | يحصل أو يضبط محاذاة النص العمودية للنص.(موروث من [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) يحصل أو يضبط عرض الإطار بوحدات 1/4000 من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | يحصل أو يضبط عرض الإطار بوحدات البكسل.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | يحصل أو يضبط عرض الإطار بوحدات نسبة مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [X](../../aspose.cells.charts/chartframe/x/) { get; set; } | (**مهمل.**) يحصل أو يضبط إحداثي س للمركّز العلوي الأيسر بوحدات 1/4000 من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | يحصل أو يضبط إحداثي x للزاوية العلوية اليسرى بوحدات البكسل.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [XRatioToChart](../../aspose.cells.charts/chartframe/xratiotochart/) { get; set; } | يحصل أو يضبط إحداثي س للمركّز العلوي الأيسر بوحدات نسبة مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y/) { get; set; } | (**مهمل.**) يحصل أو يضبط إحداثي ص للمركّز العلوي الأيسر بوحدات 1/4000 من مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | يحصل أو يضبط إحداثي y للزاوية العلوية اليسرى بوحدات البكسل.(موروث من [`ChartFrame`](../chartframe/).) |
| virtual [YRatioToChart](../../aspose.cells.charts/chartframe/yratiotochart/) { get; set; } | يحصل أو يضبط إحداثي ص للمركّز العلوي الأيسر بوحدات نسبة مساحة المخطط.(موروث من [`ChartFrame`](../chartframe/).) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | يرجع كائن Characters الذي يمثل نطاقًا من الأحرف داخل النص.(موروث من [`ChartTextFrame`](../charttextframe/).) |
| [GetLegendLabels](../../aspose.cells.charts/legend/getlegendlabels/)() | يحصل على تسميات إدخالات وسيلة الإيضاح بعد استدعاء طريقة Chart.Calculate(). |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | ضبط موضع الإطار إلى تلقائي(موروث من [`ChartFrame`](../chartframe/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class LegendDemo
    {
        public static void LegendExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // احصل على ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // الوصول إلى وسيلة الإيضاح للمخطط
            Legend legend = chart.Legend;

            // تعيين خصائص وسيلة الإيضاح
            legend.Position = LegendPositionType.Left;
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;
            legend.IsOverLay = false;
            legend.IsAutoText = true;
            legend.IsDeleted = false;
            legend.TextHorizontalAlignment = TextAlignmentType.Center;
            legend.TextVerticalAlignment = TextAlignmentType.Center;
            legend.RotationAngle = 0;
            legend.Text = "Legend Text";
            legend.LinkedSource = "Sheet1!A1";
            legend.TextDirection = TextDirectionType.LeftToRight;
            legend.ReadingOrder = TextDirectionType.Context;
            legend.DirectionType = ChartTextDirectionType.Horizontal;
            legend.IsTextWrapped = true;
            legend.IsResizeShapeToFitText = true;
            legend.IsInnerMode = false;
            legend.AutoScaleFont = true;
            legend.BackgroundMode = BackgroundMode.Transparent;
            legend.IsAutomaticSize = true;
            legend.X = 100;
            legend.Y = 100;
            legend.Height = 200;
            legend.Width = 200;
            legend.Shadow = true;

            // احفظ المصنف
            workbook.Save("LegendExample.xlsx");
            workbook.Save("LegendExample.pdf");
        }
    }
}
```

### انظر أيضًا

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


