---
title: "فئة ChartPoint"
linktitle: "ChartPoint"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ChartPoint. تغلف الكائن الذي يمثل chartpoint في Go."
type: docs
weight: 200
url: /ar/go-cpp/chartpoint/
---

## ChartPoint class

يمثل نقطة واحدة في سلسلة في مخطط.

```go

type ChartPoint struct  {
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
| [GetExplosion](./getexplosion/) | المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة. |
| [SetExplosion](./setexplosion/) | المسافة بين شريحة الفطيرة المفتوحة ومركز مخطط الفطيرة تُعبّر عنها كنسبة مئوية من قطر الفطيرة. |
| [GetShadow](./getshadow/) | True إذا كان للchartpoint ظل. |
| [SetShadow](./setshadow/) | True إذا كان للchartpoint ظل. |
| [GetBorder](./getborder/) | يحصل على Line</see>. |
| [GetArea](./getarea/) | يحصل على Area</see>. |
| [GetMarker](./getmarker/) | يحصل على Marker</see>. |
| [GetDataLabels](./getdatalabels/) | يرجع كائن DataLabels الذي يمثل تسمية البيانات المرتبطة بهذه النقطة في المخطط. |
| [Get_YValue](./get_yvalue/) | يحصل أو يعيّن قيمة Y لنقطة المخطط. |
| [SetYValue](./setyvalue/) | يحصل أو يعيّن قيمة Y لنقطة المخطط. |
| [GetYValueType](./getyvaluetype/) | يحصل على نوع قيمة Y لنقطة المخطط. |
| [GetXValue](./getxvalue/) | يحصل أو يعيّن قيمة X لنقطة المخطط. |
| [SetXValue](./setxvalue/) | يحصل أو يعيّن قيمة X لنقطة المخطط. |
| [GetXValueType](./getxvaluetype/) | يحصل على نوع قيمة X لنقطة المخطط. |
| [GetShapeProperties](./getshapeproperties/) | يحصل على كائن ShapePropertyCollection الذي يحتوي على خصائص الشكل البصرية لـ ChartPoint. |
| [IsInSecondaryPlot](./isinsecondaryplot/) | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت هذه النقطة البيانات في الشريحة الثانية أو العمود في مخطط فطيرة أو شريط من مخطط فطيرة. |
| [SetIsInSecondaryPlot](./setisinsecondaryplot/) | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت هذه النقطة البيانات في الشريحة الثانية أو العمود في مخطط فطيرة أو شريط من مخطط فطيرة. |
| [GetShapeX](./getshapex/) | يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [GetShapeY](./getshapey/) | يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [GetShapeWidth](./getshapewidth/) | يحصل على العرض بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [GetShapeHeight](./getshapeheight/) | يحصل على الارتفاع بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [GetShapeXPx](./getshapexpx/) | يحصل على إحداثي x للزاوية العلوية اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetShapeYPx](./getshapeypx/) | يحصل على إحداثي y للزاوية العلوية اليسرى بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetShapeWidthPx](./getshapewidthpx/) | يحصل على العرض بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetShapeHeightPx](./getshapeheightpx/) | يحصل على الارتفاع بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetBorderWidthPx](./getborderwidthpx/) | يحصل على عرض الحدود بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetRadiusPx](./getradiuspx/) | يحصل على نصف قطر الفقاعات أو الفطيرة أو الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetDoughnutInnerRadius](./getdoughnutinnerradius/) | يحصل على نصف القطر الداخلي لشريحة الدونات بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Doughnut. |
| [GetStartAngle](./getstartangle/) | يحصل على الزاوية الابتدائية لقسم الفطيرة، مقاسة بالدرجات في اتجاه عقارب الساعة من محور x بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Pie. |
| [GetEndAngle](./getendangle/) | يحصل على الزاوية النهائية لقسم الفطيرة، مقاسة بالدرجات في اتجاه عقارب الساعة من محور x بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Pie. |
| [GetArcStartPointXPx](./getarcstartpointxpx/) | يحصل على إحداثي x للنقطة الابتدائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات Pie و Doughnut. |
| [GetArcStartPointYPx](./getarcstartpointypx/) | يحصل على إحداثي y للنقطة الابتدائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Pie و Doughnut. |
| [GetArcEndPointXPx](./getarcendpointxpx/) | يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات Pie و Doughnut. |
| [GetArcEndPointYPx](./getarcendpointypx/) | يحصل على إحداثي y للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Pie و Doughnut. |
| [GetInnerArcStartPointXPx](./getinnerarcstartpointxpx/) | يحصل على إحداثي x للنقطة الابتدائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Doughnut. |
| [GetInnerArcStartPointYPx](./getinnerarcstartpointypx/) | يحصل على إحداثي y للنقطة الابتدائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط Doughnut. |
| [GetInnerArcEndPointXPx](./getinnerarcendpointxpx/) | يحصل على إحداثي x للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخططات الدونات. |
| [GetInnerArcEndPointYPx](./getinnerarcendpointypx/) | يحصل على إحداثي y للنقطة النهائية لقسم الفطيرة بعد استدعاء طريقة Chart.Calculate(). ينطبق على مخطط الدونات. |
| [GetTopPointCount](./gettoppointcount/) | يحصل على عدد النقاط العليا بعد استدعاء طريقة Chart.Calculate(). |
| [GetTopPointXPx](./gettoppointxpx/) | يحصل على إحداثي x للنقطة العليا للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على المخططات ثلاثية الأبعاد: Column3D, Bar3D, Cone, Cylinder, Pyramid و Area3D |
| [GetTopPointYPx](./gettoppointypx/) | يحصل على إحداثي y للنقطة العليا للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على المخططات ثلاثية الأبعاد: Column3D, Bar3D, Cone, Cylinder, Pyramid و Area3D. |
| [GetBottomPointCount](./getbottompointcount/) | يحصل على عدد النقاط السفلية بعد استدعاء طريقة Chart.Calculate(). |
| [GetBottomPointXPx](./getbottompointxpx/) | يحصل على إحداثي x للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على المخططات ثلاثية الأبعاد: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetBottomPointYPx](./getbottompointypx/) | يحصل على إحداثي y للنقطة السفلية للشكل بعد استدعاء طريقة Chart.Calculate(). ينطبق على المخططات ثلاثية الأبعاد: Column3D, Bar3D, Cone, Cylinder, Pyramid |
| [GetOnCategoryAxisPointCount](./getoncategoryaxispointcount/) | يحصل على عدد النقاط على محور الفئة بعد استدعاء طريقة Chart.Calculate(). ينطبق فقط على مخططات المنطقة. |
| [GetOnCategoryAxisPointXPx](./getoncategoryaxispointxpx/) | يحصل على إحداثي x للنقطة على محور الفئة بعد استدعاء طريقة Chart.Calculate(). ينطبق فقط على مخطط المنطقة. |
| [GetOnCategoryAxisPointYPx](./getoncategoryaxispointypx/) | يحصل على إحداثي y للنقطة على محور الفئة بعد استدعاء طريقة Chart.Calculate(). ينطبق فقط على مخطط المنطقة. |
