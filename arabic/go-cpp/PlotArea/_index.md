---
title: "PlotArea Class"
linktitle: "PlotArea"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "PlotArea class. تغلف الكائن الذي يمثل plotarea في Go."
type: docs
weight: 200
url: /ar/go-cpp/plotarea/
---

## PlotArea class

يحتوي على الكائن الذي يمثل منطقة الرسم في مخطط.

```go

type PlotArea struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewPlotArea](./newplotarea/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetXRatioToChart](./getxratiotochart/) | يحصل أو يضبط إحداثي x للزاوية العلوية اليسرى لمربع حدود مساحة الرسم كنسبة من مساحة المخطط. |
| [SetXRatioToChart](./setxratiotochart/) | يحصل أو يضبط إحداثي x للزاوية العلوية اليسرى لمربع حدود مساحة الرسم كنسبة من مساحة المخطط. |
| [GetYRatioToChart](./getyratiotochart/) | يحصل أو يضبط إحداثي y للزاوية العلوية العليا لمربع حدود plot-area كنسبة من مساحة المخطط. |
| [SetYRatioToChart](./setyratiotochart/) | يحصل أو يضبط إحداثي y للزاوية العلوية العليا لمربع حدود plot-area كنسبة من مساحة المخطط. |
| [GetHeightRatioToChart](./getheightratiotochart/) | يحصل أو يضبط ارتفاع مربع حدود مساحة الرسم بوحدات نسبة مساحة المخطط. |
| [SetHeightRatioToChart](./setheightratiotochart/) | يحصل أو يضبط ارتفاع مربع حدود مساحة الرسم بوحدات نسبة مساحة المخطط. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | يحصل أو يضبط عرض مربع حدود plot-area بوحدات نسبة مساحة المخطط. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | يحصل أو يضبط عرض مربع حدود plot-area بوحدات نسبة مساحة المخطط. |
| [GetInnerXRatioToChart](./getinnerxratiotochart/) | يحصل أو يحصل على إحداثي x للزاوية العلوية العليا لمساحة الرسم بوحدات نسبة مساحة المخطط. |
| [SetInnerXRatioToChart](./setinnerxratiotochart/) | يحصل أو يحصل على إحداثي x للزاوية العلوية العليا لمساحة الرسم بوحدات نسبة مساحة المخطط. |
| [GetInnerYRatioToChart](./getinneryratiotochart/) | يحصل أو يحصل على إحداثي x للزاوية العلوية العليا لمساحة الرسم بوحدات نسبة مساحة المخطط. |
| [SetInnerYRatioToChart](./setinneryratiotochart/) | يحصل أو يحصل على إحداثي x للزاوية العلوية العليا لمساحة الرسم بوحدات نسبة مساحة المخطط. |
| [GetInnerHeightRatioToChart](./getinnerheightratiotochart/) | يحصل أو يضبط ارتفاع مساحة الرسم بوحدات نسبة مساحة المخطط. |
| [SetInnerHeightRatioToChart](./setinnerheightratiotochart/) | يحصل أو يضبط ارتفاع مساحة الرسم بوحدات نسبة مساحة المخطط. |
| [GetInnerWidthRatioToChart](./getinnerwidthratiotochart/) | يحصل أو يعيّن عرض مساحة الرسم البياني بوحدات نسبة مساحة المخطط. |
| [SetInnerWidthRatioToChart](./setinnerwidthratiotochart/) | يحصل أو يعيّن عرض مساحة الرسم البياني بوحدات نسبة مساحة المخطط. |
| [SetPositionAuto](./setpositionauto/) | عيّن موضع مساحة الرسم إلى الوضع التلقائي |
| [IsAutomaticSize](./isautomaticsize/) | يشير إلى ما إذا كانت مساحة الرسم يتم تحجيمها تلقائيًا. |
| [SetIsAutomaticSize](./setisautomaticsize/) | يشير إلى ما إذا كانت مساحة الرسم يتم تحجيمها تلقائيًا. |
| [IsInnerMode](./isinnermode/) | يشير إلى ما إذا كان حجم مساحة الرسم يشمل علامات الفواصل وعناوين المحاور. False يحدد أن الحجم سيحدد حجم مساحة الرسم وعلامات الفواصل وعناوين المحاور. |
| [SetIsInnerMode](./setisinnermode/) | يشير إلى ما إذا كان حجم مساحة الرسم يشمل علامات الفواصل وعناوين المحاور. False يحدد أن الحجم سيحدد حجم مساحة الرسم وعلامات الفواصل وعناوين المحاور. |
| [GetShadow](./getshadow/) | True إذا كان الإطار يحتوي على ظل. |
| [SetShadow](./setshadow/) | True إذا كان الإطار يحتوي على ظل. |
| [GetShapeProperties](./getshapeproperties/) | يحصل على كائن ShapeProperties. |
| [IsDefaultPosBeSet](./isdefaultposbeset/) | يشير إلى ما إذا كان الموضع الافتراضي (DefaultX, DefaultY, DefaultWidth و DefaultHeight) مُعيّنًا. |
| [GetDefaultXRatioToChart](./getdefaultxratiotochart/) | يمثل x للموضع الافتراضي بوحدات كسر مساحة المخطط. |
| [GetDefaultYRatioToChart](./getdefaultyratiotochart/) | يمثل y للموضع الافتراضي بوحدات كسر مساحة المخطط. |
| [GetDefaultWidthRatioToChart](./getdefaultwidthratiotochart/) | يمثل عرض الموضع الافتراضي بوحدات كسر مساحة المخطط. |
| [GetDefaultHeightRatioToChart](./getdefaultheightratiotochart/) | يمثل ارتفاع الموضع الافتراضي بوحدات كسر مساحة المخطط. |
| [GetBorder](./getborder/) | يحصل على Line</see>. |
| [GetArea](./getarea/) | يحصل على Area</see>. |
| [GetTextOptions](./gettextoptions/) | يحصل أو يعيّن خيارات النص. |
| [GetFont](./getfont/) | يحصل على كائن Font لكائن ChartFrame المحدد. |
| [GetAutoScaleFont](./getautoscalefont/) | True إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True. |
| [SetAutoScaleFont](./setautoscalefont/) | True إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True. |
| [GetXPixel](./getxpixel/) | يحصل أو يعيّن إحداثي x للزاوية العلوية اليسرى بوحدات Pixel. |
| [SetXPixel](./setxpixel/) | يحصل أو يعيّن إحداثي x للزاوية العلوية اليسرى بوحدات Pixel. |
| [GetYPixel](./getypixel/) | يحصل أو يعيّن إحداثي y للزاوية العلوية اليسرى بوحدات Pixel. |
| [SetYPixel](./setypixel/) | يحصل أو يعيّن إحداثي y للزاوية العلوية اليسرى بوحدات Pixel. |
| [GetWidthPixel](./getwidthpixel/) | يحصل أو يعيّن عرض الإطار بوحدات Pixel. |
| [SetWidthPixel](./setwidthpixel/) | يحصل أو يعيّن عرض الإطار بوحدات Pixel. |
| [GetHeightPixel](./getheightpixel/) | يحصل أو يعيّن ارتفاع الإطار بوحدات Pixel. |
| [SetHeightPixel](./setheightpixel/) | يحصل أو يعيّن ارتفاع الإطار بوحدات Pixel. |
