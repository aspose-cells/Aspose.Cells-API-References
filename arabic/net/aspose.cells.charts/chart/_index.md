---
title: Chart
second_title: Aspose.Cells لمرجع .NET API
description: لتغليف الكائن الذي يمثل مخطط Excel واحدًا.
type: docs
weight: 430
url: /ar/net/aspose.cells.charts/chart/
---
## Chart class

لتغليف الكائن الذي يمثل مخطط Excel واحدًا.

```csharp
public class Chart
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling) { get; set; } | صحيح إذا قام Microsoft Excel بقياس مخطط ثلاثي الأبعاد بحيث يكون أقرب في الحجم إلى المخطط ثنائي الأبعاد المكافئ. يجب أن تكون الخاصية RightAngleAxes صحيحة. |
| [BackWall](../../aspose.cells.charts/chart/backwall) { get; } | إرجاع أ[`Walls`](./walls) يمثل الجدار الخلفي لمخطط ثلاثي الأبعاد . |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis) { get; } | الحصول على المحور X في الرسم البياني . |
| [ChartArea](../../aspose.cells.charts/chart/chartarea) { get; } | الحصول على منطقة المخطط في ورقة العمل. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable) { get; } | يمثل جدول بيانات الرسم البياني . |
| [ChartObject](../../aspose.cells.charts/chart/chartobject) { get; } | يمثل الرسم البياني الشكل ؛ |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent) { get; set; } | يمثل عمق مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 20 و 2000 بالمائة). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank) { get; set; } | يشير إلى ما إذا كان يتم عرض # N / A كقيمة فارغة. |
| [Elevation](../../aspose.cells.charts/chart/elevation) { get; set; } | يمثل ارتفاع عرض الرسم البياني ثلاثي الأبعاد بالدرجات. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle) { get; set; } | الحصول على أو تحديد زاوية المخطط الدائري الأول أو شريحة المخطط الدائري المجوف بالدرجات (باتجاه عقارب الساعة من الوضع الرأسي). ينطبق فقط على المخططات الدائرية والدائرية ثلاثية الأبعاد والدائرية المجوفة ، من 0 إلى 360. |
| [Floor](../../aspose.cells.charts/chart/floor) { get; } | إرجاع أ[`Floor`](./floor) كائن يمثل جدران مخطط ثلاثي الأبعاد . |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth) { get; set; } | الحصول على المسافة بين سلسلة البيانات في مخطط ثلاثي الأبعاد أو تعيينها ، كنسبة مئوية من عرض العلامة. يجب أن تكون قيمة هذه الخاصية بين 0 و 500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth) { get; set; } | إرجاع أو تعيين المسافة بين مجموعات الشريط أو العمود ، كنسبة مئوية من عرض الشريط أو العمود . يجب أن تكون قيمة هذه الخاصية بين 0 و 500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent) { get; set; } | إرجاع أو تعيين ارتفاع مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 5 و 500 بالمائة) . |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons) { get; set; } | يشير إلى ما إذا كان يتم إخفاء أزرار حقل المخطط المحوري فقط عندما يكون المخطط PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d) { get; } | يشير إلى ما إذا كان الرسم البياني هو مخطط ثلاثي الأبعاد . |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت منطقة الرسم البياني مستطيلة الشكل. القيمة الافتراضية هي true . |
| [Legend](../../aspose.cells.charts/chart/legend) { get; } | الحصول على وسيلة إيضاح الرسم البياني . |
| [Line](../../aspose.cells.charts/chart/line) { get; } | يحصل على الخط . |
| [Name](../../aspose.cells.charts/chart/name) { get; set; } | الحصول على اسم المخطط وتعيينه. |
| [NSeries](../../aspose.cells.charts/chart/nseries) { get; } | يحصل على أ[`SeriesCollection`](../seriescollection) مجموعة تمثل سلسلة البيانات في الرسم البياني. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup) { get; } | يمثل وصف إعداد الصفحة في هذا المخطط. |
| [Perspective](../../aspose.cells.charts/chart/perspective) { get; set; } | إرجاع أو تعيين المنظور لطريقة عرض المخطط ثلاثي الأبعاد. يجب أن تكون بين 0 و 100. يتم تجاهل هذه الخاصية إذا كانت الخاصية RightAngleAxes هي True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions) { get; } | يحدد عناصر التحكم المحورية التي تظهر في المخطط |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource) { get; set; } | المصدر هو بيانات pivotTable . إذا لم يكن PivotSource فارغًا ، فسيكون المخطط PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement) { get; set; } | يمثل طريقة إرفاق الرسم البياني بالخلايا الموجودة أسفله. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea) { get; } | الحصول على منطقة الرسم البياني للمخطط والتي تتضمن تسميات تجزئة المحور. |
| [PlotBy](../../aspose.cells.charts/chart/plotby) { get; } | الحصول على وتحديد ما إذا كان الرسم بواسطة الصف أو العمود. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype) { get; set; } | الحصول على كيفية رسم الخلايا الفارغة وتعيينها. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells) { get; set; } | يشير إلى ما إذا كان يتم رسم الخلايا المرئية فقط. |
| [PrintSize](../../aspose.cells.charts/chart/printsize) { get; set; } | الحصول على حجم الرسم البياني المطبوع وتعيينه. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes) { get; set; } | صحيح إذا كانت محاور الرسم البياني في زوايا قائمة. ينطبق فقط على المخططات ثلاثية الأبعاد (باستثناء المخططات الدائرية العمودية ثلاثية الأبعاد وثلاثية الأبعاد) . |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle) { get; set; } | يمثل استدارة عرض المخطط ثلاثي الأبعاد (دوران منطقة الرسم حول المحور z ، بالدرجات) . |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis) { get; } | الحصول على المحور X الثاني للرسم البياني . |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis) { get; } | الحصول على المحور ص الثاني في الرسم البياني . |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis) { get; } | الحصول على محور سلسلة الرسم البياني . |
| [Shapes](../../aspose.cells.charts/chart/shapes) { get; } | إرجاع كافة أشكال الرسم في هذا المخطط. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable) { get; set; } | الحصول على أو تعيين قيمة تشير إلى ما إذا كان الرسم البياني يعرض جدول بيانات أم لا. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend) { get; set; } | الحصول على قيمة أو تعيينها للإشارة إلى ما إذا كان سيتم عرض وسيلة إيضاح الرسم البياني أم لا. الافتراضي هو الصحيح. |
| [SideWall](../../aspose.cells.charts/chart/sidewall) { get; } | إرجاع أ[`Walls`](./walls)يمثل الجدار الجانبي لمخطط ثلاثي الأبعاد . |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow) { get; set; } | صحيح إذا قام Microsoft Excel بتغيير حجم المخطط ليلائم حجم نافذة ورقة المخطط. |
| [Style](../../aspose.cells.charts/chart/style) { get; set; } | الحصول على النمط المدمج وتحديده. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle) { get; } | الحصول على العنوان الفرعي للرسم البياني . فقط لملف تنسيق ODS . |
| [Title](../../aspose.cells.charts/chart/title) { get; } | الحصول على عنوان الرسم البياني . |
| [Type](../../aspose.cells.charts/chart/type) { get; set; } | الحصول على نوع الرسم البياني أو تحديده. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis) { get; } | الحصول على المحور ص في الرسم البياني . |
| [Walls](../../aspose.cells.charts/chart/walls) { get; } | إرجاع أ[`Walls`](./walls) كائن يمثل جدران مخطط ثلاثي الأبعاد . |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d) { get; set; } | صحيح إذا تم رسم خطوط الشبكة ثنائية الأبعاد على مخطط ثلاثي الأبعاد. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet) { get; } | الحصول على ورقة العمل التي تحتوي على هذا الرسم البياني . |

## طُرق

| اسم | وصف |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate)() | حساب الموضع المخصص لمنطقة قطعة الأرض ، والمحاور إذا تم تعيين موضعها تلقائيًا. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize)() | الحصول على الحجم الفعلي للرسم البياني بوحدة البكسل . |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange)() | يحصل على نطاق مصدر البيانات للمخطط. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis)(AxisType, bool) | إرجاع المحاور الموجودة على الرسم البياني. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged)() | يكتشف ما إذا كان مصدر بيانات الرسم البياني قد تغير. |
| [Move](../../aspose.cells.charts/chart/move)(int, int, int, int) | نقل الرسم البياني إلى مكان محدد . |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata)() | تحديث بيانات الرسم البياني المحوري من مصدر البيانات المحوري. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange)(string, bool) | يحدد نطاق البيانات للرسم البياني . |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn)() | مفاتيح الصف / العمود . |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage)() | يحصل على 32 بت`نقطية` كائن من الرسم البياني . |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_1)(ImageOrPrintOptions) | يحصل على 32 بت`نقطية` كائن من الرسم البياني . `خيارات ImageOrPrintOptions. تنسيق الصورة` و ImageOrPrintOptions.TiffCompression و ImageOrPrintOptions. يتم تجاهل سمات الجودة. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_6)(string) | ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_3)(Stream, ImageOrPrintOptions) | لإنشاء صورة المخطط وحفظها في دفق بالتنسيق المحدد. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_2)(Stream, ImageType) | لإنشاء صورة المخطط وحفظها في دفق بالتنسيق المحدد. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_4)(Stream, long) | لإنشاء صورة المخطط وحفظها في تدفق بتنسيق Jpeg . |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_8)(string, ImageOrPrintOptions) | ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_7)(string, ImageType) | لإنشاء صورة الرسم البياني وحفظها في ملف من نوع الصورة المحدد. |
| [ToImage](../../aspose.cells.charts/chart/toimage#toimage_9)(string, long) | لإنشاء صورة المخطط وحفظها في ملف بتنسيق Jpeg . |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf)(Stream) | لإنشاء مخطط pdf وحفظه في تيار . |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_2)(string) | يحفظ الرسم البياني في ملف pdf . |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | لإنشاء مخطط pdf وحفظه في تيار . |
| [ToPdf](../../aspose.cells.charts/chart/topdf#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | يحفظ الرسم البياني في ملف pdf . |

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
chart.ShowLegend = true;
chart.Title.Text = "Income Analysis";

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
chart.ShowLegend = True
chart.Title.Text = "Income Analysis"
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.Charts](../../aspose.cells.charts)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
