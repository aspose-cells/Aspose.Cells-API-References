---
title: "فئة SparklineGroup"
linktitle: "SparklineGroup"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة SparklineGroup. تغلف الكائن الذي يمثل sparklinegroup في Go."
type: docs
weight: 200
url: /ar/go-cpp/sparklinegroup/
---

## SparklineGroup class

<see cref=\"Sparkline\"/> يتم تنظيمه في مجموعة sparkline. مجموعة SparklineGroup تحتوي على عدد متغير من عناصر sparkline. مجموعة sparkline تحدد النوع وإعدادات العرض وإعدادات المحور للـ sparklines.

```go

type SparklineGroup struct  {
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
| [ResetRanges](./resetranges/) | يعيد تعيين نطاق البيانات ونطاق الموقع لمجموعة sparkline. هذه الطريقة ستمسح عناصر sparkline الأصلية في المجموعة وتُنشئ عناصر sparkline جديدة للنطاقات الجديدة. |
| [GetPresetStyle](./getpresetstyle/) | يحصل على ويضبط نوع نمط الإعداد المسبق لمجموعة sparkline. |
| [SetPresetStyle](./setpresetstyle/) | يحصل على ويضبط نوع نمط الإعداد المسبق لمجموعة sparkline. |
| [GetSparklines](./getsparklines/) | يحصل على مجموعة كائنات Sparkline. |
| [GetType](./gettype/) | يشير إلى نوع sparkline لمجموعة sparkline. |
| [SetType](./settype/) | يشير إلى نوع sparkline لمجموعة sparkline. |
| [GetPlotEmptyCellsType](./getplotemptycellstype/) | يشير إلى كيفية رسم الخلايا الفارغة. |
| [SetPlotEmptyCellsType](./setplotemptycellstype/) | يشير إلى كيفية رسم الخلايا الفارغة. |
| [GetDisplayHidden](./getdisplayhidden/) | يشير إلى ما إذا كان يجب عرض البيانات في الصفوف والأعمدة المخفية. |
| [SetDisplayHidden](./setdisplayhidden/) | يشير إلى ما إذا كان يجب عرض البيانات في الصفوف والأعمدة المخفية. |
| [GetShowHighPoint](./getshowhighpoint/) | يشير إلى ما إذا كان يجب تمييز أعلى نقاط البيانات في مجموعة sparkline. |
| [SetShowHighPoint](./setshowhighpoint/) | يشير إلى ما إذا كان يجب تمييز أعلى نقاط البيانات في مجموعة sparkline. |
| [GetHighPointColor](./gethighpointcolor/) | يحصل على ويضبط لون أعلى نقاط البيانات في مجموعة sparkline. |
| [SetHighPointColor](./sethighpointcolor/) | يحصل على ويضبط لون أعلى نقاط البيانات في مجموعة sparkline. |
| [GetShowLowPoint](./getshowlowpoint/) | يشير إلى ما إذا كان يجب تمييز أدنى نقاط البيانات في مجموعة sparkline. |
| [SetShowLowPoint](./setshowlowpoint/) | يشير إلى ما إذا كان يجب تمييز أدنى نقاط البيانات في مجموعة sparkline. |
| [GetLowPointColor](./getlowpointcolor/) | يحصل على ويضبط لون أدنى نقاط البيانات في مجموعة sparkline. |
| [SetLowPointColor](./setlowpointcolor/) | يحصل على ويضبط لون أدنى نقاط البيانات في مجموعة sparkline. |
| [GetShowNegativePoints](./getshownegativepoints/) | يشير إلى ما إذا كان يجب تمييز القيم السلبية في مجموعة sparkline بلون أو علامة مختلفة. |
| [SetShowNegativePoints](./setshownegativepoints/) | يشير إلى ما إذا كان يجب تمييز القيم السلبية في مجموعة sparkline بلون أو علامة مختلفة. |
| [GetNegativePointsColor](./getnegativepointscolor/) | يحصل على ويضبط لون القيم السلبية في مجموعة sparkline. |
| [SetNegativePointsColor](./setnegativepointscolor/) | يحصل على ويضبط لون القيم السلبية في مجموعة sparkline. |
| [GetShowFirstPoint](./getshowfirstpoint/) | يشير إلى ما إذا كان يجب تمييز النقطة الأولى للبيانات في مجموعة sparkline. |
| [SetShowFirstPoint](./setshowfirstpoint/) | يشير إلى ما إذا كان يجب تمييز النقطة الأولى للبيانات في مجموعة sparkline. |
| [GetFirstPointColor](./getfirstpointcolor/) | يحصل على ويضبط لون النقطة الأولى للبيانات في مجموعة sparkline. |
| [SetFirstPointColor](./setfirstpointcolor/) | يحصل على ويضبط لون النقطة الأولى للبيانات في مجموعة sparkline. |
| [GetShowLastPoint](./getshowlastpoint/) | يشير إلى ما إذا كان يجب تمييز النقطة الأخيرة للبيانات في مجموعة sparkline. |
| [SetShowLastPoint](./setshowlastpoint/) | يشير إلى ما إذا كان يجب تمييز النقطة الأخيرة للبيانات في مجموعة sparkline. |
| [GetLastPointColor](./getlastpointcolor/) | يحصل على ويضبط لون النقطة الأخيرة للبيانات في مجموعة sparkline. |
| [SetLastPointColor](./setlastpointcolor/) | يحصل على ويضبط لون النقطة الأخيرة للبيانات في مجموعة sparkline. |
| [GetShowMarkers](./getshowmarkers/) | يشير إلى ما إذا كان يجب تمييز كل نقطة في كل sparkline خطي في مجموعة sparkline. |
| [SetShowMarkers](./setshowmarkers/) | يشير إلى ما إذا كان يجب تمييز كل نقطة في كل sparkline خطي في مجموعة sparkline. |
| [GetMarkersColor](./getmarkerscolor/) | يحصل على ويضبط لون النقاط في كل sparkline خطي في مجموعة sparkline. |
| [SetMarkersColor](./setmarkerscolor/) | يحصل على ويضبط لون النقاط في كل sparkline خطي في مجموعة sparkline. |
| [GetSeriesColor](./getseriescolor/) | يحصل على ويضبط لون sparklines في مجموعة sparkline. |
| [SetSeriesColor](./setseriescolor/) | يحصل على ويضبط لون sparklines في مجموعة sparkline. |
| [GetPlotRightToLeft](./getplotrighttoleft/) | يشير إلى ما إذا كان رسم البيانات من اليمين إلى اليسار. |
| [SetPlotRightToLeft](./setplotrighttoleft/) | يشير إلى ما إذا كان رسم البيانات من اليمين إلى اليسار. |
| [GetLineWeight](./getlineweight/) | يحصل على ويضبط وزن الخط في كل sparkline خطي في مجموعة sparkline، بوحدة النقاط. |
| [SetLineWeight](./setlineweight/) | يحصل على ويضبط وزن الخط في كل sparkline خطي في مجموعة sparkline، بوحدة النقاط. |
| [GetHorizontalAxisColor](./gethorizontalaxiscolor/) | يحصل على اللون ويضبطه للمحور الأفقي في مجموعة المخططات الصغيرة. |
| [SetHorizontalAxisColor](./sethorizontalaxiscolor/) | يحصل على اللون ويضبطه للمحور الأفقي في مجموعة المخططات الصغيرة. |
| [GetShowHorizontalAxis](./getshowhorizontalaxis/) | يشير إلى ما إذا كان يجب إظهار المحور الأفقي للمخطط الصغير. يظهر المحور الأفقي إذا كان للمخطط الصغير بيانات تتقاطع مع محور الصفر. |
| [SetShowHorizontalAxis](./setshowhorizontalaxis/) | يشير إلى ما إذا كان يجب إظهار المحور الأفقي للمخطط الصغير. يظهر المحور الأفقي إذا كان للمخطط الصغير بيانات تتقاطع مع محور الصفر. |
| [GetHorizontalAxisDateRange](./gethorizontalaxisdaterange/) | يمثل النطاق الذي يحتوي على قيم التاريخ لبيانات المخطط الصغير. |
| [SetHorizontalAxisDateRange](./sethorizontalaxisdaterange/) | يمثل النطاق الذي يحتوي على قيم التاريخ لبيانات المخطط الصغير. |
| [GetVerticalAxisMaxValueType](./getverticalaxismaxvaluetype/) | يمثل نوع القيمة القصوى للمحور العمودي. |
| [SetVerticalAxisMaxValueType](./setverticalaxismaxvaluetype/) | يمثل نوع القيمة القصوى للمحور العمودي. |
| [GetVerticalAxisMaxValue](./getverticalaxismaxvalue/) | يحصل على القيمة القصوى المخصصة للمحور العمودي ويضبطها. |
| [SetVerticalAxisMaxValue_Double](./setverticalaxismaxvalue_double/) | يحصل على القيمة القصوى المخصصة للمحور العمودي ويضبطها. |
| [SetVerticalAxisMaxValue_SparklineAxisMinMaxType_Double](./setverticalaxismaxvalue_sparklineaxisminmaxtype_double/) | يضبط القيمة القصوى المخصصة للمحور العمودي للمخطط الصغير بالنوع المحدد لقيمة المحور. |
| [SetVerticalAxisMinValue_SparklineAxisMinMaxType_Double](./setverticalaxisminvalue_sparklineaxisminmaxtype_double/) | يضبط القيمة الدنيا المخصصة للمحور العمودي للمخطط الصغير بالنوع المحدد لقيمة المحور. |
| [GetVerticalAxisMinValueType](./getverticalaxisminvaluetype/) | يمثل نوع القيمة الدنيا للمحور العمودي. |
| [SetVerticalAxisMinValueType](./setverticalaxisminvaluetype/) | يمثل نوع القيمة الدنيا للمحور العمودي. |
| [GetVerticalAxisMinValue](./getverticalaxisminvalue/) | يحصل على القيمة الدنيا المخصصة للمحور العمودي ويضبطها. |
| [SetVerticalAxisMinValue_Double](./setverticalaxisminvalue_double/) | يحصل على القيمة الدنيا المخصصة للمحور العمودي ويضبطها. |
