---
title: "فئة Top10"
linktitle: "Top10"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Top10. تغلف الكائن الذي يمثل top10 في Go."
type: docs
weight: 200
url: /ar/go-cpp/top10/
---

## Top10 class

صف قاعدة التنسيق الشرطي Top10. تقوم هذه القاعدة بتنسيق الخلايا التي تقع قيمها في الفئة العليا N أو الفئة السفلى N، كما هو محدد.

```go

type Top10 struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewTop10](./newtop10/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [IsPercent](./ispercent/) | احصل أو اضبط ما إذا كانت قاعدة "top/bottom n" هي قاعدة "top/bottom n percent".القيمة الافتراضية هي false. |
| [SetIsPercent](./setispercent/) | احصل أو اضبط ما إذا كانت قاعدة "top/bottom n" هي قاعدة "top/bottom n percent".القيمة الافتراضية هي false. |
| [IsBottom](./isbottom/) | احصل أو اضبط ما إذا كانت قاعدة "top/bottom n" هي قاعدة "bottom n".القيمة الافتراضية هي false. |
| [SetIsBottom](./setisbottom/) | احصل أو اضبط ما إذا كانت قاعدة "top/bottom n" هي قاعدة "bottom n".القيمة الافتراضية هي false. |
| [GetRank](./getrank/) | احصل أو اضبط قيمة "n" في قاعدة تنسيق شرطي "top/bottom n".إذا كان IsPercent صحيحًا، يجب أن تكون القيمة بين 0 و 100.إلا يجب أن تكون بين 0 و 1000.القيمة الافتراضية هي 10. |
| [SetRank](./setrank/) | احصل أو اضبط قيمة "n" في قاعدة تنسيق شرطي "top/bottom n".إذا كان IsPercent صحيحًا، يجب أن تكون القيمة بين 0 و 100.إلا يجب أن تكون بين 0 و 1000.القيمة الافتراضية هي 10. |
