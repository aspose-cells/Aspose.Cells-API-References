---
title: Legend
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف الكائن الذي يمثل وسيلة إيضاح الرسم البياني.
type: docs
weight: 690
url: /ar/net/aspose.cells.charts/legend/
---
## Legend class

لتغليف الكائن الذي يمثل وسيلة إيضاح الرسم البياني.

```csharp
public class Legend : ChartTextFrame
```

## الخصائص

| اسم | وصف |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | يحصل على ملف[`منطقة`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | True إذا كان النص الموجود في الكائن يغير حجم الخط عندما يتغير حجم الكائن. القيمة الافتراضية هي الحقيقية. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | الحصول على وضبط وضع عرض الخلفية |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | يحصل على ملف[`الحدود`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | يمثل ارتفاع الموضع الافتراضي |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | يمثل عرض الموضع الافتراضي |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | يمثل x الوضع الافتراضي |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | يمثل y الوضع الافتراضي |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype) { get; set; } | الحصول على اتجاه النص وتحديده. |
| virtual [Font](../../aspose.cells.charts/chartframe/font) { get; } | يحصل على أ[`Font`](../chartframe/font) كائن كائن ChartFrame المحدد . |
| virtual [Height](../../aspose.cells.charts/chartframe/height) { get; set; } | الحصول على أو تحديد ارتفاع الإطار بوحدات 1/4000 من منطقة المخطط . |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | يشير إلى ما إذا كان حجم إطار المخطط تلقائيًا. |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext) { get; set; } | يشير إلى أن النص تم إنشاؤه تلقائيًا . |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | يشير إلى ما إذا كان قد تم تعيين الموضع الافتراضي (الافتراضي X ، الافتراضي Y ، العرض الافتراضي والارتفاع الافتراضي). |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted) { get; set; } | يشير إلى ما إذا كان قد تم حذف تسميات البيانات هذه. |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | يشير إلى ما إذا كان حجم مساحة قطعة الأرض يتضمن علامات التجزئة ، وتسميات المحور. |
| [IsOverLay](../../aspose.cells.charts/legend/isoverlay) { get; set; } | الحصول على أو تحديد ما إذا كان يُسمح لعناصر المخطط الأخرى بالتداخل مع عنصر المخطط هذا. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext) { get; set; } | الحصول على أو تحديد ما إذا كان يجب أن يكون الشكل مناسبًا تلقائيًا لاحتواء النص الموصوف بداخله بالكامل. الملاءمة التلقائية is عندما يتم قياس النص داخل الشكل بحيث يحتوي على كل النص الموجود بالداخل. |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان النص ملفوفًا. |
| [LegendEntries](../../aspose.cells.charts/legend/legendentries) { get; } | الحصول على مجموعة من كافة الكائنات LegendEntry في وسيلة إيضاح الرسم البياني المحددة. تعيين إدخالات وسيلة الإيضاح في المخطط السطحي غير مدعوم. |
| [LegendEntriesLabels](../../aspose.cells.charts/legend/legendentrieslabels) { get; } | يحصل على تسميات إدخالات وسيلة الإيضاح بعد استدعاء Chart.Calculate طريقة . |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource) { get; set; } | الحصول على مرجع إلى ورقة العمل وتعيينه. |
| [Position](../../aspose.cells.charts/legend/position) { get; set; } | الحصول على نوع موضع وسيلة الإيضاح أو تعيينه. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder) { get; set; } | يمثل ترتيب قراءة النص. |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle) { get; set; } | يمثل زاوية دوران النص. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | صحيح إذا كان للإطار ظل. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | يحصل على ملف[`ShapeProperties`](../chartframe/shapeproperties) الكائن . |
| virtual [Text](../../aspose.cells.charts/charttextframe/text) { get; set; } | الحصول على نص عنوان الإطار أو تحديده. |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment) { get; set; } | الحصول على المحاذاة الأفقية للنص وتعيينها. |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment) { get; set; } | الحصول على أو تعيين المحاذاة الرأسية للنص. |
| virtual [Width](../../aspose.cells.charts/chartframe/width) { get; set; } | الحصول على أو تحديد عرض الإطار بوحدات 1/4000 من منطقة المخطط . |
| virtual [X](../../aspose.cells.charts/chartframe/x) { get; set; } | الحصول على أو تحديد إحداثيات x للركن الأيسر العلوي بوحدات 1/4000 من منطقة المخطط . |
| virtual [Y](../../aspose.cells.charts/chartframe/y) { get; set; } | الحصول على أو تحديد إحداثيات y للركن الأيسر العلوي بوحدات 1/4000 من منطقة المخطط. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters)(int, int) | إرجاع كائن أحرف يمثل نطاقًا من الأحرف داخل النص. |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | ضبط موضع الإطار على Automatic |

### أمثلة

```csharp
[C#]
   
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];

Cells cells = sheet.Cells;
cells[0,1].PutValue("Income");
cells[1,0].PutValue("Company A");
cells[2,0].PutValue("Company B");
cells[3,0].PutValue("Company C");
cells[1,1].PutValue(10000);
cells[2,1].PutValue(20000);
cells[3,1].PutValue(30000);
		
int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
Chart chart = sheet.Charts[chartIndex];
chart.SetChartDataRange("A1:B4", true);
// تعيين عرض وارتفاع الأسطورة
Legend legend = chart.Legend;

// توجد وسيلة الإيضاح في الجانب الأيمن من الرسم البياني افتراضيًا.
// إذا كانت وسيلة الإيضاح في الجانب الأيسر أو الأيمن من المخطط ، فلن يتم تفعيل تعيين خاصية Legend.X.
// إذا كانت وسيلة الإيضاح في الجانب العلوي أو السفلي من المخطط ، فلن يتم تفعيل خاصية Legend.Y.
legend.Y = 1500;
legend.Width = 50;
legend.Height = 50; 
// تعيين موقف الأسطورة
legend.Position = LegendPositionType.Left;

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim sheet as Worksheet = workbook.Worksheets(0)

Dim cells as Cells = sheet.Cells
cells(0,1).PutValue("Income")
cells(1,0).PutValue("Company A")
cells(2,0).PutValue("Company B")
cells(3,0).PutValue("Company C")
cells(1,1).PutValue(10000)
cells(2,1).PutValue(20000)
cells(3,1).PutValue(30000)
		
Dim chartIndex as Integer = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15)

Dim chart as Chart = sheet.Charts(chartIndex)
chart.SetChartDataRange("A1:B4", True);
 
'Set Legend's width and height
Dim legend as Legend = chart.Legend

'توجد وسيلة الإيضاح في الجانب الأيمن من الرسم البياني افتراضيًا.
'إذا كانت وسيلة الإيضاح على الجانب الأيسر أو الأيمن من المخطط ، فلن يتم تفعيل تعيين خاصية Legend.X.
'إذا كانت وسيلة الإيضاح في الجانب العلوي أو السفلي من المخطط ، فلن يتم تفعيل خاصية Legend.Y.
legend.Y = 1500
legend.Width = 50
legend.Height = 50
'Set legend's position
legend.Position = LegendPositionType.Left
```

### أنظر أيضا

* class [ChartTextFrame](../charttextframe)
* مساحة الاسم [Aspose.Cells.Charts](../../aspose.cells.charts)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
