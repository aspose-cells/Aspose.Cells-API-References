---
title: "فئة ShapePath"
linktitle: "ShapePath"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ShapePath. تغلف الكائن الذي يمثل shapepath في Go."
type: docs
weight: 200
url: /ar/go-cpp/shapepath/
---

## ShapePath class

يمثل مسار إنشاء يتكون من سلسلة من الحركات والخطوط والمنحنيات التي عند دمجها ستشكل شكلاً هندسياً.

```go

type ShapePath struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewShapePath](./newshapepath/) | يُنشئ مثيلًا جديدًا من فئة ShapePath. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetPathSegments](./getpathsegments/) | يحصل على قائمة ShapeSegmentPathCollection |
| [GetWidthPixel](./getwidthpixel/) | يحصل على عرض هذا المسار بوحدة البكسل. |
| [SetWidthPixel](./setwidthpixel/) | يحصل على عرض هذا المسار بوحدة البكسل. |
| [GetHeightPixel](./getheightpixel/) | يحصل على ارتفاع هذا المسار بوحدة البكسل. |
| [SetHeightPixel](./setheightpixel/) | يحصل على ارتفاع هذا المسار بوحدة البكسل. |
| [MoveTo](./moveto/) | يبدأ شكلًا جديدًا من النقطة المحددة دون إغلاق الشكل الحالي. جميع النقاط اللاحقة التي تُضاف إلى المسار تُضاف إلى هذا الشكل الجديد. الوحدة: بكسل. |
| [LineTo](./lineto/) | يضيف مقطع خط إلى الشكل الحالي. النقطة البداية هي نقطة النهاية للشكل الحالي. الوحدة: بكسل. |
| [CubicBezierTo](./cubicbezierto/) | يضيف منحنى بيزيه مكعب إلى الشكل الحالي. النقطة البداية هي نقطة النهاية للشكل الحالي. الوحدة: بكسل. |
| [ArcTo](./arcto/) | يضيف قوسًا بيضاويًا إلى الشكل الحالي. النقطة البداية هي نقطة النهاية للشكل الحالي. |
| [Close](./close/) | يغلق الشكل الحالي ويبدأ شكلًا جديدًا. إذا كان الشكل الحالي يحتوي على سلسلة من الخطوط والمنحنيات المتصلة، فإن الطريقة تغلق الحلقة بربط خط من نقطة النهاية إلى نقطة البداية. |
