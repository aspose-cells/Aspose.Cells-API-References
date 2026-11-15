---
title: "الفئة ReferredArea"
linktitle: "ReferredArea"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "الفئة ReferredArea. تغلف الكائن الذي يمثل referredarea في Go."
type: docs
weight: 200
url: /ar/go-cpp/referredarea/
---

## ReferredArea class

يمثل المنطقة المشار إليها بواسطة الصيغة.

```go

type ReferredArea struct  {
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
| [IsExternalLink](./isexternallink/) | يشير إلى ما إذا كان هذا رابطًا خارجيًا. |
| [GetExternalFileName](./getexternalfilename/) | احصل على اسم الملف الخارجي إذا كان هذا إشارة خارجية. |
| [GetSheetName](./getsheetname/) | يشير إلى الورقة التي توجد فيها هذه الإشارة. |
| [GetSheetNames](./getsheetnames/) | أسماء جميع أوراق العمل التي تشير إليها هذه المثيلة. |
| [IsEntireRow](./isentirerow/) | يشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الأعمدة (صف كامل). |
| [IsEntireColumn](./isentirecolumn/) | يشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الصفوف (عمود كامل). |
| [IsArea](./isarea/) | يشير إلى ما إذا كانت هذه منطقة. |
| [GetEndColumn](./getendcolumn/) | العمود النهائي للمنطقة. |
| [GetStartColumn](./getstartcolumn/) | عمود البداية للمنطقة. |
| [GetEndRow](./getendrow/) | صف النهاية للمنطقة. |
| [GetStartRow](./getstartrow/) | صف البداية للمنطقة. |
| [GetValues](./getvalues/) | يحصل على قيم الخلايا في هذه المنطقة. |
| [GetValues_Bool](./getvalues_bool/) | يحصل على قيم الخلايا في هذه المنطقة. |
| [GetValue_Int_Int](./getvalue_int_int/) | يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة. |
| [GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة. |
| [ToString](./tostring/) | يرجع عنوان المرجع لهذه المنطقة. عادةً يكون عنوان المرجع الذي يمكن استخدامه في الصيغة، مثل "Sheet1!A1:C3". |
