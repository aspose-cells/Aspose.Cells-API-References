---
title: "فئة Walls"
linktitle: "Walls"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Walls. تغلف الكائن الذي يمثل الجدران في Go."
type: docs
weight: 200
url: /ar/go-cpp/walls/
---

## Walls class

يحتوي على الكائن الذي يمثل جدران مخطط ثلاثي الأبعاد.

```go

type Walls struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewWalls](./newwalls/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetCenterX](./getcenterx/) | يحصل على إحداثي x للزاوية اليسرى السفلية لمركز Wall بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [GetCenterY](./getcentery/) | يحصل على إحداثي y للزاوية اليسرى السفلية لمركز Wall بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [GetWidth](./getwidth/) | يحصل على العرض من اليسار إلى اليمين بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [GetDepth](./getdepth/) | يحصل على العمق من الأمام إلى الخلف بوحدات 1/4000 من عرض المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [GetHeight](./getheight/) | يحصل على الارتفاع من الأعلى إلى الأسفل بوحدات 1/4000 من ارتفاع المخطط بعد استدعاء طريقة Chart.Calculate(). |
| [GetCenterXPx](./getcenterxpx/) | يحصل على إحداثي x للزاوية السفلية اليسرى لمركز Wall بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetCenterYPx](./getcenterypx/) | يحصل على إحداثي y للزاوية اليسرى السفلية لمركز Wall بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetWidthPx](./getwidthpx/) | يحصل على العرض من اليسار إلى اليمين بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetDepthPx](./getdepthpx/) | يحصل على العمق من الأمام إلى الخلف بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetHeightPx](./getheightpx/) | يحصل على الارتفاع من الأعلى إلى الأسفل بوحدات البكسل بعد استدعاء طريقة Chart.Calculate(). |
| [GetCubePointCount](./getcubepointcount/) | يحصل على عدد نقاط المكعب بعد استدعاء طريقة Chart.Calculate(). |
| [GetCubePointXPx](./getcubepointxpx/) | يحصل على إحداثي x لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). عدد نقاط القمة لمكعب الجدران هو ثمانية |
| [GetCubePointYPx](./getcubepointypx/) | يحصل على إحداثي y لنقطة القمة لمكعب الجدران بعد استدعاء طريقة Chart.Calculate(). عدد نقاط القمة لمكعب الجدران هو ثمانية. |
| [GetBackgroundColor](./getbackgroundcolor/) | يحصل أو يضبط لون الخلفية للمنطقة. |
| [SetBackgroundColor](./setbackgroundcolor/) | يحصل أو يضبط لون الخلفية للمنطقة. |
| [GetForegroundColor](./getforegroundcolor/) | يحصل أو يضبط لون المقدمة. |
| [SetForegroundColor](./setforegroundcolor/) | يحصل أو يضبط لون المقدمة. |
| [GetFormatting](./getformatting/) | يمثل تنسيق المنطقة. |
| [SetFormatting](./setformatting/) | يمثل تنسيق المنطقة. |
| [GetInvertIfNegative](./getinvertifnegative/) | إذا كانت الخاصية صحيحة وكانت قيمة نقطة المخطط عددًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية. |
| [SetInvertIfNegative](./setinvertifnegative/) | إذا كانت الخاصية صحيحة وكانت قيمة نقطة المخطط عددًا سالبًا، سيتم تبادل لون المقدمة ولون الخلفية. |
| [GetFillFormat](./getfillformat/) | يمثل كائن FillFormat الذي يحتوي على خصائص تنسيق التعبئة للمخطط أو الشكل المحدد. |
| [GetTransparency](./gettransparency/) | يرجع أو يضبط درجة شفافية المنطقة كقيمة تتراوح من 0.0 (معتم) إلى 1.0 (شفاف). |
| [SetTransparency](./settransparency/) | يرجع أو يضبط درجة شفافية المنطقة كقيمة تتراوح من 0.0 (معتم) إلى 1.0 (شفاف). |
| [GetBorder](./getborder/) | يحصل أو يضبط خط الحدود. |
| [SetBorder](./setborder/) | يحصل أو يضبط خط الحدود. |
