---
title: "فئة SeriesCollection"
linktitle: "SeriesCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "الفئة SeriesCollection. تغلف الكائن الذي يمثل seriescollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/seriescollection/
---

## SeriesCollection class

يحتوي على مجموعة من كائنات <see cref=\"Series\"/>.

```go

type SeriesCollection struct  {
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
| [Get](./get/) | يحصل على عنصر Series في الفهرس المحدد. |
| [GetSeriesByOrder](./getseriesbyorder/) | يحصل على عنصر Series حسب الترتيب. |
| [RemoveAt](./removeat/) | إزالة السلسلة عند الفهرس المحدد. |
| [GetCategoryData](./getcategorydata/) | يحصل أو يضبط نطاق قيم محور الفئة. يمكن أن يكون نطاق خلايا (مثل \"d1:e10\") أو تسلسل قيم (مثل \"{2,6,8,10}\"). |
| [SetCategoryData](./setcategorydata/) | يحصل أو يضبط نطاق قيم محور الفئة. يمكن أن يكون نطاق خلايا (مثل \"d1:e10\") أو تسلسل قيم (مثل \"{2,6,8,10}\"). |
| [GetSecondCategoryData](./getsecondcategorydata/) | يحصل أو يضبط نطاق قيم محور الفئة الثاني. يمكن أن يكون نطاق خلايا (مثل \"d1:e10\"), أو تسلسل قيم (مثل \"{2,6,8,10}\"). يؤثر فقط عندما يتم رسم بعض السلاسل على المحور الثاني. |
| [SetSecondCategoryData](./setsecondcategorydata/) | يحصل أو يضبط نطاق قيم محور الفئة الثاني. يمكن أن يكون نطاق خلايا (مثل \"d1:e10\"), أو تسلسل قيم (مثل \"{2,6,8,10}\"). يؤثر فقط عندما يتم رسم بعض السلاسل على المحور الثاني. |
| [SwapSeries](./swapseries/) | يغيّر مباشرة ترتيب السلسلتين. |
| [SetSeriesNames](./setseriesnames/) | يضبط أسماء جميع السلاسل في المخطط. |
| [AddR1C1](./addr1c1/) | يضيف مجموعة Series إلى مخطط. |
| [Add_String_Bool](./add_string_bool/) | يضيف مجموعة Series إلى مخطط. |
| [Add_String_Bool_Bool](./add_string_bool_bool/) | يضيف مجموعة Series إلى مخطط. |
| [IsColorVaried](./iscolorvaried/) | يمثل ما إذا كان لون النقاط متنوعًا. |
| [SetIsColorVaried](./setiscolorvaried/) | يمثل ما إذا كان لون النقاط متنوعًا. |
| [Clear](./clear/) | يمسح المجموعة |
| [ChangeColors](./changecolors/) | ضبط لوحة ألوان أحادية اللون لسلسلة المخطط. |
| [GetCount](./getcount/) | يحصل على عدد العناصر الموجودة في المثيل. |
