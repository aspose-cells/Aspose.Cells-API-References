---
title: "فئة Name"
linktitle: "Name"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Name. تغلف الكائن الذي يمثل name في Go."
type: docs
weight: 200
url: /ar/go-cpp/name/
---

## Name class

يمثل اسمًا معرفًا لنطاق من الخلايا.

```go

type Name struct  {
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
| [GetComment](./getcomment/) | يحصل على ويضبط تعليق الاسم. ينطبق فقط على Excel 2007 أو الإصدارات الأحدث. |
| [SetComment](./setcomment/) | يحصل على ويضبط تعليق الاسم. ينطبق فقط على Excel 2007 أو الإصدارات الأحدث. |
| [GetText](./gettext/) | يحصل على نص الاسم للكائن. |
| [SetText](./settext/) | يحصل على نص الاسم للكائن. |
| [GetFullText](./getfulltext/) | يحصل على النص الكامل للاسم للكائن مع إعداد النطاق. |
| [GetRefersTo](./getrefersto/) | إرجاع أو تعيين الصيغة التي يُعرّف الاسم للإشارة إليها، وتبدأ بعلامة مساواة. |
| [SetRefersTo_String](./setrefersto_string/) | إرجاع أو تعيين الصيغة التي يُعرّف الاسم للإشارة إليها، وتبدأ بعلامة مساواة. |
| [GetR1C1RefersTo](./getr1c1refersto/) | الحصول على أو تعيين مرجع R1C1 للاسم. |
| [SetR1C1RefersTo](./setr1c1refersto/) | الحصول على أو تعيين مرجع R1C1 للاسم. |
| [GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | احصل على مرجع هذا الاسم. |
| [GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | احصل على مرجع هذا الاسم بناءً على الخلية المحددة. |
| [SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | تعيين مرجع هذا الاسم. |
| [IsReferred](./isreferred/) | يشير إلى ما إذا كان هذا الاسم مُشارًا إليه من قبل صيغ أخرى. |
| [IsVisible](./isvisible/) | يشير إلى ما إذا كان الاسم مرئيًا. |
| [SetIsVisible](./setisvisible/) | يشير إلى ما إذا كان الاسم مرئيًا. |
| [GetSheetIndex](./getsheetindex/) | يشير إلى أن هذا الاسم ينتمي إلى المصنف أو ورقة العمل. 0 = اسم عالمي، وإلا فالمؤشر إلى الورقة (بدءًا من الواحد). |
| [SetSheetIndex](./setsheetindex/) | يشير إلى أن هذا الاسم ينتمي إلى المصنف أو ورقة العمل. 0 = اسم عالمي، وإلا فالمؤشر إلى الورقة (بدءًا من الواحد). |
| [ToString](./tostring/) | يرجع سلسلة تمثل كائن Range الحالي. |
| [GetRanges](./getranges/) | الحصول على جميع النطاقات التي يُشير إليها هذا الاسم. |
| [GetRanges_Bool](./getranges_bool/) | الحصول على جميع النطاقات التي يُشير إليها هذا الاسم. |
| [GetReferredAreas](./getreferredareas/) | الحصول على جميع المراجع التي يُشير إليها هذا الاسم. |
| [GetRange](./getrange/) | الحصول على النطاق إذا كان هذا الاسم يشير إلى نطاق. |
| [GetRange_Bool](./getrange_bool/) | الحصول على النطاق إذا كان هذا الاسم يشير إلى نطاق |
| [GetRange_Int_Int_Int](./getrange_int_int_int/) | الحصول على النطاق إذا كان هذا الاسم يشير إلى نطاق. إذا لم يكن مرجع هذا الاسم مطلقًا، قد يختلف النطاق بين الخلايا المختلفة. |
