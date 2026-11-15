---
title: "فئة ChartFrame"
linktitle: "ChartFrame"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ChartFrame. تغلف الكائن الذي يمثل chartframe في Go."
type: docs
weight: 200
url: /ar/go-cpp/chartframe/
---

## ChartFrame class

يغلف الكائن الذي يمثل كائن الإطار في مخطط.

```go

type ChartFrame struct  {
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
| [IsAutomaticSize](./isautomaticsize/) | يشير إلى ما إذا كان إطار المخطط مُحَدَّد تلقائيًا. |
| [SetIsAutomaticSize](./setisautomaticsize/) | يشير إلى ما إذا كان إطار المخطط مُحَدَّد تلقائيًا. |
| [GetXRatioToChart](./getxratiotochart/) | يحصل أو يضبط إحداثي x للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط. |
| [SetXRatioToChart](./setxratiotochart/) | يحصل أو يضبط إحداثي x للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط. |
| [GetYRatioToChart](./getyratiotochart/) | يحصل أو يعيّن إحداثي y للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط. |
| [SetYRatioToChart](./setyratiotochart/) | يحصل أو يعيّن إحداثي y للزاوية العلوية اليسرى بوحدات نسبة مساحة المخطط. |
| [GetWidthRatioToChart](./getwidthratiotochart/) | يحصل أو يعيّن عرض الإطار بوحدات نسبة مساحة المخطط. |
| [SetWidthRatioToChart](./setwidthratiotochart/) | يحصل أو يعيّن عرض الإطار بوحدات نسبة مساحة المخطط. |
| [GetHeightRatioToChart](./getheightratiotochart/) | يحصل أو يعيّن ارتفاع الإطار بوحدات نسبة مساحة المخطط. |
| [SetHeightRatioToChart](./setheightratiotochart/) | يحصل أو يعيّن ارتفاع الإطار بوحدات نسبة مساحة المخطط. |
| [GetXPixel](./getxpixel/) | يحصل أو يعيّن إحداثي x للزاوية العلوية اليسرى بوحدات Pixel. |
| [SetXPixel](./setxpixel/) | يحصل أو يعيّن إحداثي x للزاوية العلوية اليسرى بوحدات Pixel. |
| [GetYPixel](./getypixel/) | يحصل أو يعيّن إحداثي y للزاوية العلوية اليسرى بوحدات Pixel. |
| [SetYPixel](./setypixel/) | يحصل أو يعيّن إحداثي y للزاوية العلوية اليسرى بوحدات Pixel. |
| [GetWidthPixel](./getwidthpixel/) | يحصل أو يعيّن عرض الإطار بوحدات Pixel. |
| [SetWidthPixel](./setwidthpixel/) | يحصل أو يعيّن عرض الإطار بوحدات Pixel. |
| [GetHeightPixel](./getheightpixel/) | يحصل أو يعيّن ارتفاع الإطار بوحدات Pixel. |
| [SetHeightPixel](./setheightpixel/) | يحصل أو يعيّن ارتفاع الإطار بوحدات Pixel. |
| [SetPositionAuto](./setpositionauto/) | تعيين موضع الإطار إلى تلقائي |
