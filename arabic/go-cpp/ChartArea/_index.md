---
title: "فئة ChartArea"
linktitle: "ChartArea"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ChartArea. تغلف الكائن الذي يمثل chartarea في Go."
type: docs
weight: 200
url: /ar/go-cpp/chartarea/
---

## ChartArea class

يغلف الكائن الذي يمثل منطقة المخطط في ورقة العمل.

```go

type ChartArea struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewChartArea](./newchartarea/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetXRatioToChart](./getxratiotochart/) | يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، كنسبة من مساحة المخطط. |
| [SetXRatioToChart](./setxratiotochart/) | يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية العلوية اليسرى، كنسبة من مساحة المخطط. |
| [GetYRatioToChart](./getyratiotochart/) | يحصل أو يضبط الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات النسبة من مساحة المخطط. |
| [SetYRatioToChart](./setyratiotochart/) | يحصل أو يضبط الإزاحة العمودية من صف الزاوية العلوية اليسرى، بوحدات النسبة من مساحة المخطط. |
| [GetHeightRatioToChart](./getheightratiotochart/) | يحصل أو يضبط الإزاحة العمودية من صف الزاوية السفلية اليمنى، بوحدات النسبة من مساحة المخطط. |
| [SetHeightRatioToChart](./setheightratiotochart/) | يحصل أو يضبط الإزاحة العمودية من صف الزاوية السفلية اليمنى، بوحدات النسبة من مساحة المخطط. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات النسبة من مساحة المخطط. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | يحصل أو يضبط الإزاحة الأفقية من عمود الزاوية السفلية اليمنى، بوحدات النسبة من مساحة المخطط. |
| [GetFont](./getfont/) | يحصل على كائن Font للكيان ChartArea المحدد. |
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
| [GetAutoScaleFont](./getautoscalefont/) | True إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True. |
| [SetAutoScaleFont](./setautoscalefont/) | True إذا كان النص في الكائن يغيّر حجم الخط عندما يتغيّر حجم الكائن. القيمة الافتراضية هي True. |
| [IsAutomaticSize](./isautomaticsize/) | يشير إلى ما إذا كان إطار المخطط مُحَدَّد تلقائيًا. |
| [SetIsAutomaticSize](./setisautomaticsize/) | يشير إلى ما إذا كان إطار المخطط مُحَدَّد تلقائيًا. |
| [GetXPixel](./getxpixel/) | يحصل أو يعيّن إحداثي x للزاوية العلوية اليسرى بوحدات Pixel. |
| [SetXPixel](./setxpixel/) | يحصل أو يعيّن إحداثي x للزاوية العلوية اليسرى بوحدات Pixel. |
| [GetYPixel](./getypixel/) | يحصل أو يعيّن إحداثي y للزاوية العلوية اليسرى بوحدات Pixel. |
| [SetYPixel](./setypixel/) | يحصل أو يعيّن إحداثي y للزاوية العلوية اليسرى بوحدات Pixel. |
| [GetWidthPixel](./getwidthpixel/) | يحصل أو يعيّن عرض الإطار بوحدات Pixel. |
| [SetWidthPixel](./setwidthpixel/) | يحصل أو يعيّن عرض الإطار بوحدات Pixel. |
| [GetHeightPixel](./getheightpixel/) | يحصل أو يعيّن ارتفاع الإطار بوحدات Pixel. |
| [SetHeightPixel](./setheightpixel/) | يحصل أو يعيّن ارتفاع الإطار بوحدات Pixel. |
| [SetPositionAuto](./setpositionauto/) | تعيين موضع الإطار إلى تلقائي |
