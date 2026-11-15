---
title: "فئة Chart"
linktitle: "Chart"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Chart. يغلف الكائن الذي يمثل chart في Go."
type: docs
weight: 200
url: /ar/go-cpp/chart/
---

## Chart class

يغلف الكائن الذي يمثل مخطط Excel واحد.

```go

type Chart struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetStyle](./getstyle/) | يحصل ويضبط النمط المدمج. |
| [SetStyle](./setstyle/) | يحصل ويضبط النمط المدمج. |
| [GetChartObject](./getchartobject/) | يمثل chartShape؛ |
| [GetHidePivotFieldButtons](./gethidepivotfieldbuttons/) | يشير إلى ما إذا كان يجب إخفاء أزرار حقول المخطط المحوري فقط عندما يكون المخطط PivotChart. |
| [SetHidePivotFieldButtons](./sethidepivotfieldbuttons/) | يشير إلى ما إذا كان يجب إخفاء أزرار حقول المخطط المحوري فقط عندما يكون المخطط PivotChart. |
| [GetPivotOptions](./getpivotoptions/) | يحدد عناصر التحكم المحورية التي تظهر على المخطط. |
| [GetPivotSource](./getpivotsource/) | المصدر هو بيانات جدول المحور. إذا لم يكن PivotSource فارغًا، فإن المخطط هو PivotChart. |
| [SetPivotSource](./setpivotsource/) | المصدر هو بيانات جدول المحور. إذا لم يكن PivotSource فارغًا، فإن المخطط هو PivotChart. |
| [IsCellReferedByChart](./iscellreferedbychart/) | يعيد ما إذا كانت الخلية المشار إليها بواسطة المخطط. |
| [IsChartDataChanged](./ischartdatachanged/) | يكشف ما إذا كان مصدر بيانات المخطط قد تغير. |
| [GetPlotBy](./getplotby/) | يحصل ويضبط ما إذا كان الرسم حسب الصف أو العمود. |
| [RefreshPivotData](./refreshpivotdata/) | يقوم بتحديث بيانات المخطط من جدول المحور. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | يحصل ويضبط طريقة رسم الخلايا الفارغة. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | يحصل ويضبط طريقة رسم الخلايا الفارغة. |
| [GetPlotVisibleCellsOnly](./getplotvisiblecellsonly/) | يشير إلى ما إذا كان يجب رسم الخلايا المرئية فقط. |
| [SetPlotVisibleCellsOnly](./setplotvisiblecellsonly/) | يشير إلى ما إذا كان يجب رسم الخلايا المرئية فقط. |
| [GetDisplayNaAsBlank](./getdisplaynaasblank/) | يشير إلى ما إذا كان يجب عرض #N/A كقيمة فارغة. |
| [SetDisplayNaAsBlank](./setdisplaynaasblank/) | يشير إلى ما إذا كان يجب عرض #N/A كقيمة فارغة. |
| [GetName](./getname/) | يحصل ويضبط اسم المخطط. |
| [SetName](./setname/) | يحصل ويضبط اسم المخطط. |
| [GetSizeWithWindow](./getsizewithwindow/) | صحيح إذا كان Microsoft Excel يعيد تحجيم المخطط ليتطابق مع حجم نافذة ورقة المخطط. |
| [SetSizeWithWindow](./setsizewithwindow/) | صحيح إذا كان Microsoft Excel يعيد تحجيم المخطط ليتطابق مع حجم نافذة ورقة المخطط. |
| [GetWorksheet](./getworksheet/) | يحصل على ورقة العمل التي تحتوي على هذا المخطط. |
| [GetShapes](./getshapes/) | يعيد جميع أشكال الرسم في هذا المخطط. |
| [GetPrintSize](./getprintsize/) | يحصل ويضبط حجم المخطط المطبوع. |
| [SetPrintSize](./setprintsize/) | يحصل ويضبط حجم المخطط المطبوع. |
| [ChangeTemplate](./changetemplate/) | غيّر نوع المخطط باستخدام قالب مسبق. |
| [GetType](./gettype/) | يحصل أو يضبط نوع المخطط. |
| [SetType](./settype/) | يحصل أو يضبط نوع المخطط. |
| [Move](./move/) | ينقل المخطط إلى موقع محدد. |
| [GetNSeries](./getnseries/) | يحصل على مجموعة SeriesCollection التي تمثل سلاسل البيانات في المخطط. |
| [GetFilteredNSeries](./getfilterednseries/) | يحصل على مجموعة SeriesCollection التي تمثل سلاسل البيانات التي تم تصفيتها في المخطط. |
| [GetTitle](./gettitle/) | يحصل على عنوان المخطط. |
| [GetSubTitle](./getsubtitle/) | يحصل على العنوان الفرعي للمخطط. ينطبق فقط على ملفات ODS. |
| [GetPlotArea](./getplotarea/) | يحصل على مساحة الرسم للمخطط التي تشمل تسميات علامات المحور. |
| [GetChartArea](./getchartarea/) | يحصل على مساحة المخطط في ورقة العمل. |
| [GetCategoryAxis](./getcategoryaxis/) | يحصل على محور X للمخطط. |
| [GetValueAxis](./getvalueaxis/) | يحصل على محور Y للمخطط. |
| [GetSecondValueAxis](./getsecondvalueaxis/) | يحصل على المحور Y الثاني للمخطط. |
| [GetSecondCategoryAxis](./getsecondcategoryaxis/) | يحصل على المحور X الثاني للمخطط. |
| [GetSeriesAxis](./getseriesaxis/) | يحصل على محور السلاسل للمخطط. |
| [GetLegend](./getlegend/) | يحصل على مفتاح المخطط. |
| [GetChartDataTable](./getchartdatatable/) | يمثل جدول بيانات المخطط. |
| [GetShowLegend](./getshowlegend/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان مفتاح المخطط سيُعرض. القيمة الافتراضية هي true. |
| [SetShowLegend](./setshowlegend/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان مفتاح المخطط سيُعرض. القيمة الافتراضية هي true. |
| [IsRectangularCornered](./isrectangularcornered/) | يحصل أو يضبط قيمة تشير إلى ما إذا كانت مساحة المخطط ذات زوايا مستطيلة. القيمة الافتراضية هي true. |
| [SetIsRectangularCornered](./setisrectangularcornered/) | يحصل أو يضبط قيمة تشير إلى ما إذا كانت مساحة المخطط ذات زوايا مستطيلة. القيمة الافتراضية هي true. |
| [GetShowDataTable](./getshowdatatable/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان المخطط يعرض جدول بيانات. |
| [SetShowDataTable](./setshowdatatable/) | يحصل أو يضبط قيمة تشير إلى ما إذا كان المخطط يعرض جدول بيانات. |
| [GetFirstSliceAngle](./getfirstsliceangle/) | يحصل أو يضبط زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، ومخططات الدونات، من 0 إلى 360. |
| [SetFirstSliceAngle](./setfirstsliceangle/) | يحصل أو يضبط زاوية الشريحة الأولى في مخطط الفطيرة أو مخطط الدونات، بالدرجات (مع اتجاه عقارب الساعة من العمودي). ينطبق فقط على مخططات الفطيرة، الفطيرة ثلاثية الأبعاد، ومخططات الدونات، من 0 إلى 360. |
| [GetGapWidth](./getgapwidth/) | يعيد أو يضبط المسافة بين مجموعات الأعمدة أو الأعمدة، كنسبة مئوية من عرض العمود أو الشريط. يجب أن تكون قيمة هذه الخاصية بين 0 و 500. |
| [SetGapWidth](./setgapwidth/) | يعيد أو يضبط المسافة بين مجموعات الأعمدة أو الأعمدة، كنسبة مئوية من عرض العمود أو الشريط. يجب أن تكون قيمة هذه الخاصية بين 0 و 500. |
| [GetGapDepth](./getgapdepth/) | يحصل أو يضبط المسافة بين سلاسل البيانات في مخطط ثلاثي الأبعاد، كنسبة مئوية من عرض العلامة. يجب أن تكون قيمة هذه الخاصية بين 0 و 500. |
| [SetGapDepth](./setgapdepth/) | يحصل أو يضبط المسافة بين سلاسل البيانات في مخطط ثلاثي الأبعاد، كنسبة مئوية من عرض العلامة. يجب أن تكون قيمة هذه الخاصية بين 0 و 500. |
| [Calculate](./calculate/) | يحسب المواضع المخصصة لمساحة الرسم والمحاور إذا تم تعيين مواضعها تلقائيًا. |
| [Calculate_ChartCalculateOptions](./calculate_chartcalculateoptions/) | يحسب الموضع المخصص لمنطقة الرسم والمحاور إذا تم تعيين موضعها تلقائيًا، باستخدام خيارات حساب المخطط. |
| [GetFloor](./getfloor/) | يرجع كائن Floor الذي يمثل جدران مخطط ثلاثي الأبعاد. |
| [GetWalls](./getwalls/) | يرجع كائن Walls الذي يمثل جدران مخطط ثلاثي الأبعاد. |
| [GetBackWall](./getbackwall/) | يرجع كائن Walls الذي يمثل الجدار الخلفي لمخطط ثلاثي الأبعاد. |
| [GetSideWall](./getsidewall/) | يرجع كائن Walls الذي يمثل الجدار الجانبي لمخطط ثلاثي الأبعاد. |
| [GetWallsAndGridlines2D](./getwallsandgridlines2d/) | صحيح إذا تم رسم خطوط الشبكة ثنائي الأبعاد على مخطط ثلاثي الأبعاد. |
| [SetWallsAndGridlines2D](./setwallsandgridlines2d/) | صحيح إذا تم رسم خطوط الشبكة ثنائي الأبعاد على مخطط ثلاثي الأبعاد. |
| [GetRotationAngle](./getrotationangle/) | يمثل دوران عرض المخطط ثلاثي الأبعاد (دوران منطقة الرسم حول المحور z، بالدرجات). |
| [SetRotationAngle](./setrotationangle/) | يمثل دوران عرض المخطط ثلاثي الأبعاد (دوران منطقة الرسم حول المحور z، بالدرجات). |
| [GetElevation](./getelevation/) | يمثل ارتفاع عرض المخطط ثلاثي الأبعاد، بالدرجات. |
| [SetElevation](./setelevation/) | يمثل ارتفاع عرض المخطط ثلاثي الأبعاد، بالدرجات. |
| [GetRightAngleAxes](./getrightangleaxes/) | صحيح إذا كانت محاور المخطط بزاوية قائمة. ينطبق فقط على المخططات ثلاثية الأبعاد (باستثناء Column3D ومخططات الفطيرة ثلاثية الأبعاد). |
| [SetRightAngleAxes](./setrightangleaxes/) | صحيح إذا كانت محاور المخطط بزاوية قائمة. ينطبق فقط على المخططات ثلاثية الأبعاد (باستثناء Column3D ومخططات الفطيرة ثلاثية الأبعاد). |
| [GetAutoScaling](./getautoscaling/) | صحيح إذا قام Microsoft Excel بتقليل حجم مخطط ثلاثي الأبعاد ليصبح أقرب في الحجم إلى المخطط الثنائي الأبعاد المقابل. يجب أن تكون خاصية RightAngleAxes صحيحة. |
| [SetAutoScaling](./setautoscaling/) | صحيح إذا قام Microsoft Excel بتقليل حجم مخطط ثلاثي الأبعاد ليصبح أقرب في الحجم إلى المخطط الثنائي الأبعاد المقابل. يجب أن تكون خاصية RightAngleAxes صحيحة. |
| [GetHeightPercent](./getheightpercent/) | يرجع أو يضبط ارتفاع مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 5 و500 بالمائة). |
| [SetHeightPercent](./setheightpercent/) | يرجع أو يضبط ارتفاع مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 5 و500 بالمائة). |
| [GetPerspective](./getperspective/) | يرجع أو يضبط منظور عرض المخطط ثلاثي الأبعاد. يجب أن يكون بين 0 و100. يتم تجاهل هذه الخاصية إذا كانت خاصية RightAngleAxes صحيحة. |
| [SetPerspective](./setperspective/) | يرجع أو يضبط منظور عرض المخطط ثلاثي الأبعاد. يجب أن يكون بين 0 و100. يتم تجاهل هذه الخاصية إذا كانت خاصية RightAngleAxes صحيحة. |
| [GetIs3D](./getis3d/) | يشير إلى ما إذا كان المخطط مخططًا ثلاثي الأبعاد. |
| [GetDepthPercent](./getdepthpercent/) | يمثل عمق مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 20 و2000 بالمائة). |
| [SetDepthPercent](./setdepthpercent/) | يمثل عمق مخطط ثلاثي الأبعاد كنسبة مئوية من عرض المخطط (بين 20 و2000 بالمائة). |
| [ToImage_String](./toimage_string/) | ينشئ صورة المخطط ويحفظها في ملف. تحدد امتداد اسم الملف صيغة الصورة. |
| [ToImage_String_ImageType](./toimage_string_imagetype/) | ينشئ صورة المخطط ويحفظها في ملف بنوع الصورة المحدد. |
| [ToImage_Int64](./toimage_int64/) | ينشئ صورة المخطط ويحفظها في تدفق بصيغة Jpeg. |
| [ToImage_ImageType](./toimage_imagetype/) | ينشئ صورة المخطط ويحفظها في تدفق بالصيفة المحددة. |
| [ToPdf_String](./topdf_string/) | يحفظ المخطط في ملف pdf. |
| [ToPdf_String_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_string_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | يحفظ المخطط في ملف pdf. |
| [ToPdf](./topdf/) | ينشئ ملف PDF للمخطط ويحفظه في تدفق. |
| [ToPdf_Float_Float_PageLayoutAlignmentType_PageLayoutAlignmentType](./topdf_float_float_pagelayoutalignmenttype_pagelayoutalignmenttype/) | ينشئ ملف pdf للمخطط ويحفظه في تدفق. |
| [ToImage_String_ImageOrPrintOptions](./toimage_string_imageorprintoptions/) | ينشئ صورة المخطط ويحفظها في ملف. تحدد امتداد اسم الملف صيغة الصورة. |
| [ToImage_ImageOrPrintOptions](./toimage_imageorprintoptions/) | ينشئ صورة المخطط ويحفظها في تدفق بالصيفة المحددة. |
| [GetActualSize](./getactualsize/) | يحصل على الحجم الفعلي للمخطط بوحدة البكسل. |
| [GetPlacement](./getplacement/) | يمثل الطريقة التي يتم بها إرفاق المخطط بالخلايا تحته. |
| [SetPlacement](./setplacement/) | يمثل الطريقة التي يتم بها إرفاق المخطط بالخلايا تحته. |
| [GetPageSetup](./getpagesetup/) | يمثل وصف إعداد الصفحة في هذا المخطط. |
| [HasAxis](./hasaxis/) | يرجع المحاور الموجودة في المخطط. |
| [SwitchRowColumn](./switchrowcolumn/) | يبدل الصف/العمود. |
| [GetChartDataRange](./getchartdatarange/) | يحصل على نطاق مصدر البيانات للمخطط. |
| [SetChartDataRange](./setchartdatarange/) | يحدد نطاق البيانات للمخطط. |
| [GetLine](./getline/) | يحصل على الخط. |
