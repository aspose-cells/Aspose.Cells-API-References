---
title: "الفئة ChartArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.ChartArea. تغلف الكائن الذي يمثل منطقة المخطط في ورقة العمل."
type: docs
url: /ar/net/aspose.cells.charts/chartarea/
---
## ChartArea class

يحتوي على الكائن الذي يمثل منطقة المخطط في ورقة العمل.

```csharp
public class ChartArea : ChartFrame
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
| override [Font](../../aspose.cells.charts/chartarea/font/) { get; } | يحصل على كائن [`Font`](./font/) لمنطقة المخطط المحددة. |
| override [Height](../../aspose.cells.charts/chartarea/height/) { get; set; } | (**Obsolete.**) يحصل أو يضبط الإزاحة العمودية من صف الزاوية السفلية‑اليمنى، بوحدات 1/4000 من منطقة المخطط. |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | الحصول على أو تعيين ارتفاع الإطار بوحدات البكسل.(مستمد من [`ChartFrame`](../chartframe/).) |
| override [HeightRatioToChart](../../aspose.cells.charts/chartarea/heightratiotochart/) { get; set; } | يحصل أو يضبط الإزاحة العمودية من صف الزاوية السفلية اليمنى، بوحدات نسبة من منطقة المخطط. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | يشير إلى ما إذا كان إطار المخطط يتم تحجيمه تلقائيًا.(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | يشير إلى ما إذا تم تعيين الموضع الافتراضي (DefaultX، DefaultY، DefaultWidth و DefaultHeight).(مستمد من [`ChartFrame`](../chartframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | يشير إلى ما إذا كان حجم مساحة الرسم البياني يشمل علامات الفواصل وعناوين المحاور. القيمة False تحدد أن الحجم سيحدد حجم مساحة الرسم البياني، وعلامات الفواصل، وعناوين المحاور.(مستمد من [`ChartFrame`](../chartframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | صحيح إذا كان للإطار ظل.(مستمد من [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | الحصول على كائن [`ShapeProperties`](../chartframe/shapeproperties/).(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) الحصول على كائن [`Font`](../chartframe/font/) لإطار ChartFrame المحدد.(مستمد من [`ChartFrame`](../chartframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | الحصول على وتعيين خيارات النص.(مستمد من [`ChartFrame`](../chartframe/).) |
| override [Width](../../aspose.cells.charts/chartarea/width/) { get; set; } | (**Obsolete.**) يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات 1/4000 من منطقة المخطط. |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | يحصل أو يضبط عرض الإطار بوحدات البكسل.(موروث من [`ChartFrame`](../chartframe/).) |
| override [WidthRatioToChart](../../aspose.cells.charts/chartarea/widthratiotochart/) { get; set; } | يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات نسبة من منطقة المخطط. |
| override [X](../../aspose.cells.charts/chartarea/x/) { get; set; } | (**Obsolete.**) يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية العليا‑اليسرى، بوحدات 1/4000 من منطقة المخطط. |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | يحصل أو يضبط إحداثي x للزاوية العلوية اليسرى بوحدات البكسل.(موروث من [`ChartFrame`](../chartframe/).) |
| override [XRatioToChart](../../aspose.cells.charts/chartarea/xratiotochart/) { get; set; } | يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية العليا اليسرى، كنسبة من منطقة المخطط. |
| override [Y](../../aspose.cells.charts/chartarea/y/) { get; set; } | (**Obsolete.**) يحصل أو يحصل على الإزاحة العمودية من صف الزاوية العليا اليسرى، بوحدات 1/4000 من منطقة المخطط. |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | يحصل أو يضبط إحداثي y للزاوية العلوية اليسرى بوحدات البكسل.(موروث من [`ChartFrame`](../chartframe/).) |
| override [YRatioToChart](../../aspose.cells.charts/chartarea/yratiotochart/) { get; set; } | يحصل أو يحصل على الإزاحة العمودية من صف الزاوية العليا اليسرى، بوحدات نسبة من منطقة المخطط. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | ضبط موضع الإطار إلى تلقائي(موروث من [`ChartFrame`](../chartframe/).) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartAreaDemo
    {
        public static void ChartAreaExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الحصول على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة قيمة عينة إلى الخلية "A1"
            worksheet.Cells["A1"].PutValue(50);

            // إضافة قيمة عينة إلى الخلية "A2"
            worksheet.Cells["A2"].PutValue(100);

            // إضافة قيمة عينة إلى الخلية "A3"
            worksheet.Cells["A3"].PutValue(150);

            // إضافة قيمة عينة إلى الخلية "B1"
            worksheet.Cells["B1"].PutValue(60);

            // إضافة قيمة عينة إلى الخلية "B2"
            worksheet.Cells["B2"].PutValue(32);

            // إضافة قيمة عينة إلى الخلية "B3"
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B3"
            chart.NSeries.Add("A1:B3", true);

            // الحصول على منطقة المخطط
            ChartArea chartArea = chart.ChartArea;

            // تعيين خصائص منطقة المخطط
            chartArea.X = 10;
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;
            chartArea.IsInnerMode = false;
            chartArea.AutoScaleFont = true;
            chartArea.BackgroundMode = BackgroundMode.Transparent;
            chartArea.IsAutomaticSize = true;
            chartArea.Shadow = true;

            // ضبط لون المقدمة لمنطقة المخطط
            chartArea.Area.ForegroundColor = Color.Yellow;

            // حفظ ملف Excel
            workbook.Save("ChartAreaExample.xlsx");
            workbook.Save("ChartAreaExample.pdf");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../chartframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


