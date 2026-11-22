---
title: "الصنف Chart"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الصنف Aspose.Cells.Charts.Chart. يغلف الكائن الذي يمثل مخطط Excel واحد."
type: docs
url: /ar/net/aspose.cells.charts/chart/
---
## Chart class

يغلف الكائن الذي يمثل مخطط Excel واحد.

```csharp
public class Chart
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActualChartSize](../../aspose.cells.charts/chart/actualchartsize/) { get; } | (**Obsolete.**) يحصل على الحجم الفعلي للمخطط بوحدات البكسل. |
| [AutoScaling](../../aspose.cells.charts/chart/autoscaling/) { get; set; } | صحيح إذا كان Microsoft Excel يقيّم مخططًا ثلاثي الأبعاد بحيث يكون حجمه أقرب إلى المخطط الثنائي الأبعاد المكافئ. يجب أن تكون الخاصية RightAngleAxes صحيحة. |
| [BackWall](../../aspose.cells.charts/chart/backwall/) { get; } | يرجع كائن [`Walls`](./walls/) الذي يمثل الجدار الخلفي لمخطط ثلاثي الأبعاد. |
| [CategoryAxis](../../aspose.cells.charts/chart/categoryaxis/) { get; } | يحصل على محور X للمخطط. |
| [ChartArea](../../aspose.cells.charts/chart/chartarea/) { get; } | يحصل على مساحة المخطط في ورقة العمل. |
| [ChartDataTable](../../aspose.cells.charts/chart/chartdatatable/) { get; } | يمثل جدول بيانات المخطط. |
| [ChartObject](../../aspose.cells.charts/chart/chartobject/) { get; } | يمثل الـ chartShape؛ |
| [DepthPercent](../../aspose.cells.charts/chart/depthpercent/) { get; set; } | يمثل عمق مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 20 و2000 في المئة). |
| [DisplayNaAsBlank](../../aspose.cells.charts/chart/displaynaasblank/) { get; set; } | يشير إلى ما إذا كان يجب عرض #N/A كقيمة فارغة. |
| [Elevation](../../aspose.cells.charts/chart/elevation/) { get; set; } | يمثل ارتفاع عرض المخطط ثلاثي الأبعاد، بالدرجات. |
| [FilteredNSeries](../../aspose.cells.charts/chart/filterednseries/) { get; } | يحصل على مجموعة [`SeriesCollection`](../seriescollection/) تمثل سلاسل البيانات التي تم تصفيتها في المخطط. |
| [FirstSliceAngle](../../aspose.cells.charts/chart/firstsliceangle/) { get; set; } | يحصل أو يعيّن زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، ومخططات الدونات، من 0 إلى 360. |
| [Floor](../../aspose.cells.charts/chart/floor/) { get; } | يعيد كائن [`Floor`](./floor/) يمثل جدران مخطط ثلاثي الأبعاد. |
| [GapDepth](../../aspose.cells.charts/chart/gapdepth/) { get; set; } | يحصل أو يعيّن المسافة بين سلاسل البيانات في مخطط ثلاثي الأبعاد، كنسبة مئوية من عرض العلامة. يجب أن تكون قيمة هذه الخاصية بين 0 و500. |
| [GapWidth](../../aspose.cells.charts/chart/gapwidth/) { get; set; } | يعيد أو يعيّن المسافة بين مجموعات الأعمدة أو الأشرطة، كنسبة مئوية من عرض العمود أو الشريط. يجب أن تكون قيمة هذه الخاصية بين 0 و500. |
| [HeightPercent](../../aspose.cells.charts/chart/heightpercent/) { get; set; } | يعيد أو يعيّن ارتفاع مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 5 و500 في المئة). |
| [HidePivotFieldButtons](../../aspose.cells.charts/chart/hidepivotfieldbuttons/) { get; set; } | يشير إلى ما إذا كان يتم إخفاء أزرار حقول مخطط المحور فقط عندما يكون المخطط PivotChart. |
| [Is3D](../../aspose.cells.charts/chart/is3d/) { get; } | يشير إلى ما إذا كان المخطط مخططًا ثلاثي الأبعاد. |
| [IsRectangularCornered](../../aspose.cells.charts/chart/isrectangularcornered/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت مساحة المخطط ذات زوايا مستطيلة. القيمة الافتراضية هي true. |
| [Legend](../../aspose.cells.charts/chart/legend/) { get; } | يحصل على مفتاح المخطط. |
| [Line](../../aspose.cells.charts/chart/line/) { get; } | يحصل على الخط. |
| [Name](../../aspose.cells.charts/chart/name/) { get; set; } | يحصل ويعيّن اسم المخطط. |
| [NSeries](../../aspose.cells.charts/chart/nseries/) { get; } | يحصل على مجموعة [`SeriesCollection`](../seriescollection/) تمثل سلاسل البيانات في المخطط. |
| [PageSetup](../../aspose.cells.charts/chart/pagesetup/) { get; } | يمثل وصف إعداد الصفحة في هذا المخطط. |
| [Perspective](../../aspose.cells.charts/chart/perspective/) { get; set; } | يعيد أو يعيّن منظور عرض المخطط ثلاث‑الأبعاد. يجب أن يكون بين 0 و100. يتم تجاهل هذه الخاصية إذا كانت الخاصية RightAngleAxes تساوي True. |
| [PivotOptions](../../aspose.cells.charts/chart/pivotoptions/) { get; } | يحدد عناصر التحكم المحورية التي تظهر على المخطط |
| [PivotSource](../../aspose.cells.charts/chart/pivotsource/) { get; set; } | المصدر هو بيانات جدول المحور. إذا لم يكن PivotSource فارغًا، يكون المخطط PivotChart. |
| [Placement](../../aspose.cells.charts/chart/placement/) { get; set; } | يمثل الطريقة التي يتم بها إرفاق المخطط بالخلايا أسفله. |
| [PlotArea](../../aspose.cells.charts/chart/plotarea/) { get; } | يحصل على مساحة رسم المخطط التي تشمل تسميات علامات المحور. |
| [PlotBy](../../aspose.cells.charts/chart/plotby/) { get; } | يحصل ويعيّن ما إذا كان الرسم حسب الصف أو العمود. |
| [PlotEmptyCellsType](../../aspose.cells.charts/chart/plotemptycellstype/) { get; set; } | يحصل ويعيّن طريقة رسم الخلايا الفارغة. |
| [PlotVisibleCells](../../aspose.cells.charts/chart/plotvisiblecells/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كان يتم عرض خلايا المخطط المرئية فقط. |
| [PlotVisibleCellsOnly](../../aspose.cells.charts/chart/plotvisiblecellsonly/) { get; set; } | يشير إلى ما إذا كان يتم عرض خلايا المخطط المرئية فقط. |
| [PrintSize](../../aspose.cells.charts/chart/printsize/) { get; set; } | يحصل على حجم المخطط المطبوع ويضبطه. |
| [RightAngleAxes](../../aspose.cells.charts/chart/rightangleaxes/) { get; set; } | صحيح إذا كانت محاور المخطط عمودية على بعضها. ينطبق فقط على المخططات ثلاثية الأبعاد (باستثناء Column3D ومخططات الفطيرة ثلاثية الأبعاد). |
| [RotationAngle](../../aspose.cells.charts/chart/rotationangle/) { get; set; } | يمثل دوران عرض المخطط ثلاثي الأبعاد (دوران منطقة المخطط حول المحور z، بالدرجات). |
| [SecondCategoryAxis](../../aspose.cells.charts/chart/secondcategoryaxis/) { get; } | يحصل على المحور X الثاني للمخطط. |
| [SecondValueAxis](../../aspose.cells.charts/chart/secondvalueaxis/) { get; } | يحصل على المحور Y الثاني للمخطط. |
| [SeriesAxis](../../aspose.cells.charts/chart/seriesaxis/) { get; } | يحصل على محور السلسلة للمخطط. |
| [Shapes](../../aspose.cells.charts/chart/shapes/) { get; } | يعيد جميع أشكال الرسم في هذا المخطط. |
| [ShowDataTable](../../aspose.cells.charts/chart/showdatatable/) { get; set; } | يحصل على أو يضبط قيمة تشير إلى ما إذا كان المخطط يعرض جدول بيانات. |
| [ShowLegend](../../aspose.cells.charts/chart/showlegend/) { get; set; } | يحصل على أو يضبط قيمة تشير إلى ما إذا كان سيتم عرض مفتاح المخطط. القيمة الافتراضية هي true. |
| [SideWall](../../aspose.cells.charts/chart/sidewall/) { get; } | يعيد كائن [`Walls`](./walls/) الذي يمثل الجدار الجانبي لمخطط ثلاثي الأبعاد. |
| [SizeWithWindow](../../aspose.cells.charts/chart/sizewithwindow/) { get; set; } | صحيح إذا كان Microsoft Excel يعيد تحجيم المخطط ليتطابق مع حجم نافذة ورقة المخطط. |
| [Style](../../aspose.cells.charts/chart/style/) { get; set; } | يحصل على النمط المدمج ويضبطه. |
| [SubTitle](../../aspose.cells.charts/chart/subtitle/) { get; } | يحصل على العنوان الفرعي للمخطط. ينطبق فقط على ملفات ODS. |
| [Title](../../aspose.cells.charts/chart/title/) { get; } | يحصل على عنوان المخطط. |
| [Type](../../aspose.cells.charts/chart/type/) { get; set; } | يحصل على أو يضبط نوع المخطط. |
| [ValueAxis](../../aspose.cells.charts/chart/valueaxis/) { get; } | يحصل على المحور Y للمخطط. |
| [Walls](../../aspose.cells.charts/chart/walls/) { get; } | يعيد كائن [`Walls`](./walls/) الذي يمثل جدران مخطط ثلاثي الأبعاد. |
| [WallsAndGridlines2D](../../aspose.cells.charts/chart/wallsandgridlines2d/) { get; set; } | صحيح إذا تم رسم خطوط الشبكة ثنائي الأبعاد على مخطط ثلاثي الأبعاد. |
| [Worksheet](../../aspose.cells.charts/chart/worksheet/) { get; } | يحصل على ورقة العمل التي تحتوي على هذا المخطط. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate)() | يحسب المواضع المخصصة لمنطقة المخطط والمحاور إذا تم تعيين مواضعها تلقائيًا. |
| [Calculate](../../aspose.cells.charts/chart/calculate/#calculate_1)(ChartCalculateOptions) | يحسب الموضع المخصص لمنطقة المخطط والمحاور إذا تم تعيين موضعها تلقائيًا، باستخدام خيارات حساب المخطط. |
| [ChangeTemplate](../../aspose.cells.charts/chart/changetemplate/)(byte[]) | غيّر نوع المخطط باستخدام قالب مسبق. |
| [GetActualSize](../../aspose.cells.charts/chart/getactualsize/)() | يحصل على الحجم الفعلي للمخطط بوحدة البكسل. |
| [GetChartDataRange](../../aspose.cells.charts/chart/getchartdatarange/)() | يحصل على نطاق مصدر البيانات للمخطط. |
| [HasAxis](../../aspose.cells.charts/chart/hasaxis/)(AxisType, bool) | يعيد أي المحاور الموجودة في المخطط. |
| [IsCellReferedByChart](../../aspose.cells.charts/chart/iscellreferedbychart/)(int, int, int) | يعيد ما إذا كانت الخلية المشار إليها من قبل المخطط. |
| [IsChartDataChanged](../../aspose.cells.charts/chart/ischartdatachanged/)() | يكشف ما إذا كان مصدر بيانات المخطط قد تغير. |
| [IsReferedByChart](../../aspose.cells.charts/chart/isreferedbychart/)(int, int) | (**Obsolete.**) يعيد ما إذا كانت الخلية مشار إليها من قبل المخطط. |
| [Move](../../aspose.cells.charts/chart/move/)(int, int, int, int) | ينقل المخطط إلى موقع محدد. |
| [RefreshPivotData](../../aspose.cells.charts/chart/refreshpivotdata/)() | يقوم بتحديث بيانات المخطط من جدول محوري. |
| [SetChartDataRange](../../aspose.cells.charts/chart/setchartdatarange/)(string, bool) | يحدد نطاق البيانات للمخطط. |
| [SwitchRowColumn](../../aspose.cells.charts/chart/switchrowcolumn/)() | يبدل الصف/العمود. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage)() | يحصل على كائن `Bitmap` 32-بت للمخطط. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_1)(ImageOrPrintOptions) | يحصل على كائن `Bitmap` 32-بت للمخطط. يتم تجاهل سمات `ImageOrPrintOptions.ImageFormat`، ImageOrPrintOptions.TiffCompression و ImageOrPrintOptions.Quality. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_6)(string) | ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_5)(Stream, ImageFormat) | (**Obsolete.**) ينشئ صورة المخطط ويحفظها في تدفق بالتنسيق المحدد. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_3)(Stream, ImageOrPrintOptions) | ينشئ صورة المخطط ويحفظها في تدفق بالتنسيق المحدد. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_2)(Stream, ImageType) | ينشئ صورة المخطط ويحفظها في تدفق بالتنسيق المحدد. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_4)(Stream, long) | ينشئ صورة المخطط ويحفظها في تدفق بتنسيق Jpeg. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_10)(string, ImageFormat) | (**Obsolete.**) ينشئ صورة المخطط ويحفظها في ملف بالتنسيق المحدد. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_8)(string, ImageOrPrintOptions) | ينشئ صورة المخطط ويحفظها في ملف. امتداد اسم الملف يحدد تنسيق الصورة. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_7)(string, ImageType) | ينشئ صورة المخطط ويحفظها في ملف بنوع الصورة المحدد. |
| [ToImage](../../aspose.cells.charts/chart/toimage/#toimage_9)(string, long) | (**Obsolete.**) ينشئ صورة المخطط ويحفظها في ملف بتنسيق Jpeg. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf)(Stream) | ينشئ ملف PDF للمخطط ويحفظه في تدفق. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_2)(string) | يحفظ المخطط في ملف pdf. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_1)(Stream, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | ينشئ ملف pdf للمخطط ويحفظه في تدفق. |
| [ToPdf](../../aspose.cells.charts/chart/topdf/#topdf_3)(string, float, float, PageLayoutAlignmentType, PageLayoutAlignmentType) | يحفظ المخطط في ملف pdf. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartDemo
    {
        public static void ChartExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells[0, 1].PutValue("Income");
            worksheet.Cells[1, 0].PutValue("Company A");
            worksheet.Cells[2, 0].PutValue("Company B");
            worksheet.Cells[3, 0].PutValue("Company C");
            worksheet.Cells[1, 1].PutValue(10000);
            worksheet.Cells[2, 1].PutValue(20000);
            worksheet.Cells[3, 1].PutValue(30000);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // تحديد نطاق البيانات للمخطط
            chart.SetChartDataRange("A1:B4", true);

            // تعيين خصائص المخطط
            chart.ShowLegend = true;
            chart.Title.Text = "Income Analysis";
            chart.Style = 2; // Built-in style

            // تخصيص مظهر المخطط
            chart.ChartObject.Name = "IncomeChart";
            chart.PlotEmptyCellsType = PlotEmptyCellsType.NotPlotted;
            chart.PlotVisibleCells = true;
            chart.DisplayNaAsBlank = true;
            chart.SizeWithWindow = true;

            // تخصيص محاور المخطط
            chart.CategoryAxis.Title.Text = "Companies";
            chart.ValueAxis.Title.Text = "Income";
            chart.CategoryAxis.MajorTickMark = TickMarkType.Outside;
            chart.ValueAxis.MajorTickMark = TickMarkType.Outside;

            // تخصيص وسيلة إيضاح المخطط
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.IsOverLay = false;

            // تخصيص منطقة رسم المخطط
            chart.PlotArea.Area.ForegroundColor = Color.LightYellow;
            chart.PlotArea.Border.IsVisible = false;

            // تخصيص منطقة مخطط الرسم
            chart.ChartArea.Area.ForegroundColor = Color.LightBlue;
            chart.ChartArea.Border.IsVisible = false;

            // احفظ المصنف
            workbook.Save("ChartExample.xlsx");
            workbook.Save("ChartExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


