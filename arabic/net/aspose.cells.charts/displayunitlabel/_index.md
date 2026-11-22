---
title: "الفئة DisplayUnitLabel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Charts.DisplayUnitLabel. تمثل تسمية وحدة العرض"
type: docs
url: /ar/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

يمثل تسمية وحدة العرض.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | يحصل على [`area`](../chartframe/area/).(موروث من [`ChartFrame`](../chartframe/).) |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont/) { get; set; } | صحيح إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True. |
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
| override [Font](../../aspose.cells.charts/displayunitlabel/font/) { get; } | يحصل على كائن [`Font`](./font/) للإطار المخطط (ChartFrame) المحدد. |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) الحصول على أو تعيين ارتفاع الإطار بوحدات 1/4000 من مساحة المخطط.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | الحصول على أو تعيين ارتفاع الإطار بوحدات البكسل.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | الحصول على أو تعيين ارتفاع الإطار بوحدات نسبة مساحة المخطط.(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | يشير إلى ما إذا كان نص المخطط يدور تلقائيًا.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | يشير إلى ما إذا كان إطار المخطط يتم تحجيمه تلقائيًا.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext/) { get; set; } | يشير إلى أن النص يتم إنشاؤه تلقائيًا.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | يشير إلى ما إذا تم تعيين الموضع الافتراضي (DefaultX، DefaultY، DefaultWidth و DefaultHeight).(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | يشير إلى ما إذا تم حذف تسمية البيانات هذه.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | يشير إلى ما إذا كان حجم مساحة الرسم البياني يشمل علامات الفواصل وعناوين المحاور. القيمة False تحدد أن الحجم سيحدد حجم مساحة الرسم البياني، وعلامات الفواصل، وعناوين المحاور.(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | الحصول على أو تعيين ما إذا كان يجب أن يتناسب الشكل تلقائيًا لاحتواء النص الموصوف بداخله بالكامل. التناسب التلقائي هو عندما يتم تحجيم النص داخل الشكل لاحتواء جميع النص داخل الشكل.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped/) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان النص مكسورًا.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | الحصول على وتعيين إشارة إلى ورقة العمل.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | يمثل ترتيب قراءة النص.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | يمثل زاوية دوران النص.(مستمد من [`ChartTextFrame`](../charttextframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | صحيح إذا كان للإطار ظل.(مستمد من [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | الحصول على كائن [`ShapeProperties`](../chartframe/shapeproperties/).(مستمد من [`ChartFrame`](../chartframe/).) |
| override [Text](../../aspose.cells.charts/displayunitlabel/text/) { get; set; } | يحصل أو يضبط نص تسمية وحدة العرض. |
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
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | ضبط موضع الإطار إلى تلقائي(موروث من [`ChartFrame`](../chartframe/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DisplayUnitLabelDemo
    {
        public static void DisplayUnitLabelExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            // إضافة ورقة عمل جديدة إلى كائن Workbook
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

            // ضبط وحدة العرض للمحور القيمي (Y)
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // ضبط خصائص DisplayUnitLabel
            displayUnitLabel.Text = "100";
            displayUnitLabel.AutoScaleFont = true;
            displayUnitLabel.IsAutoText = false;
            displayUnitLabel.IsDeleted = false;
            displayUnitLabel.TextHorizontalAlignment = TextAlignmentType.Center;
            displayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;
            displayUnitLabel.RotationAngle = 0;
            displayUnitLabel.LinkedSource = "";
            displayUnitLabel.TextDirection = TextDirectionType.LeftToRight;
            displayUnitLabel.ReadingOrder = TextDirectionType.LeftToRight;
            displayUnitLabel.DirectionType = ChartTextDirectionType.Horizontal;
            displayUnitLabel.IsTextWrapped = false;
            displayUnitLabel.IsResizeShapeToFitText = false;
            displayUnitLabel.IsInnerMode = false;
            displayUnitLabel.BackgroundMode = BackgroundMode.Transparent;
            displayUnitLabel.IsAutomaticSize = true;
            displayUnitLabel.X = 0;
            displayUnitLabel.Y = 0;
            displayUnitLabel.Height = 100;
            displayUnitLabel.Width = 100;
            displayUnitLabel.Shadow = false;

            // حفظ ملف Excel
            workbook.Save("DisplayUnitLabelExample.xlsx");
            workbook.Save("DisplayUnitLabelExample.pdf");
        }
    }
}
```

### انظر أيضًا

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


