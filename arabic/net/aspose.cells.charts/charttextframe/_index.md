---
title: "Class ChartTextFrame"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Charts.ChartTextFrame. تغلف الكائن الذي يمثل كائن الإطار الذي يحتوي على النص"
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/
---
## ChartTextFrame class

يحتوي على الكائن الذي يمثل كائن الإطار الذي يحتوي على النص.

```csharp
public class ChartTextFrame : ChartFrame
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
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype/) { get; set; } | يحصل على اتجاه النص ويضبطه. |
| virtual [Font](../../aspose.cells.charts/chartframe/font/) { get; } | الحصول على كائن [`Font`](../chartframe/font/) لإطار ChartFrame المحدد.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) الحصول على أو تعيين ارتفاع الإطار بوحدات 1/4000 من مساحة المخطط.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | الحصول على أو تعيين ارتفاع الإطار بوحدات البكسل.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | الحصول على أو تعيين ارتفاع الإطار بوحدات نسبة مساحة المخطط.(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | يشير إلى ما إذا كان نص المخطط يتم تدويره تلقائيًا. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | يشير إلى ما إذا كان إطار المخطط يتم تحجيمه تلقائيًا.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext/) { get; set; } | يشير إلى أن النص تم إنشاؤه تلقائيًا. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | يشير إلى ما إذا تم تعيين الموضع الافتراضي (DefaultX، DefaultY، DefaultWidth و DefaultHeight).(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | يشير إلى ما إذا كان هذا التسمية البيانية محذوفة. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | يشير إلى ما إذا كان حجم مساحة الرسم البياني يشمل علامات الفواصل وعناوين المحاور. القيمة False تحدد أن الحجم سيحدد حجم مساحة الرسم البياني، وعلامات الفواصل، وعناوين المحاور.(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | يحصل أو يحدد ما إذا كان يجب أن يتناسب الشكل تلقائيًا لاحتواء النص الموصوف بداخله بالكامل. التناسب التلقائي هو عندما يتم تحجيم النص داخل الشكل لتضمين كل النص داخل. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped/) { get; set; } | يحصل على أو يضبط قيمة تشير إلى ما إذا كان النص مُلتفًا. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | يحصل ويحدد مرجعًا إلى ورقة العمل. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | يمثل ترتيب قراءة النص. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | يمثل زاوية تدوير النص. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | صحيح إذا كان للإطار ظل.(مستمد من [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | الحصول على كائن [`ShapeProperties`](../chartframe/shapeproperties/).(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [Text](../../aspose.cells.charts/charttextframe/text/) { get; set; } | يحصل أو يحدد نص عنوان الإطار. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) يمثل ترتيب قراءة النص. |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) الحصول على كائن [`Font`](../chartframe/font/) لإطار ChartFrame المحدد.(مستمد من [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | يحصل ويحدد محاذاة النص أفقياً. |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | الحصول على وتعيين خيارات النص.(مستمد من [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | يحصل أو يحدد محاذاة النص عمودياً. |
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
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | يرجع كائن Characters الذي يمثل نطاقًا من الأحرف داخل النص. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | ضبط موضع الإطار إلى تلقائي(موروث من [`ChartFrame`](../chartframe/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class ChartTextFrameDemo
    {
        public static void ChartTextFrameExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
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

            // إضافة سلسلة إلى المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى عنوان المخطط
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
            title.TextHorizontalAlignment = TextAlignmentType.Center;
            title.TextVerticalAlignment = TextAlignmentType.Center;
            title.RotationAngle = 0;
            title.IsAutoText = false;
            title.IsDeleted = false;
            title.TextDirection = TextDirectionType.LeftToRight;
            title.ReadingOrder = TextDirectionType.LeftToRight;
            title.DirectionType = ChartTextDirectionType.Horizontal;
            title.IsTextWrapped = true;
            title.IsResizeShapeToFitText = true;
            title.IsInnerMode = false;
            title.AutoScaleFont = true;
            title.BackgroundMode = BackgroundMode.Transparent;
            title.IsAutomaticSize = true;
            title.X = 0;
            title.Y = 0;
            title.Height = 400;
            title.Width = 400;
            title.Shadow = true;

            // احفظ المصنف
            workbook.Save("ChartTextFrameExample.xlsx");
            workbook.Save("ChartTextFrameExample.pdf");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../chartframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


