---
title: "CopyOptions فئة"
linktitle: "CopyOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "CopyOptions فئة. يغلف الكائن الذي يمثل copyoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/copyoptions/
---

## CopyOptions class

يمثل خيارات النسخ.

```go

type CopyOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewCopyOptions](./newcopyoptions/) | CopyOptions منشئ. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetKeepMacros](./getkeepmacros/) | يشير إلى ما إذا كان يتم الاحتفاظ بالماكرو؛ |
| [SetKeepMacros](./setkeepmacros/) | يشير إلى ما إذا كان يتم الاحتفاظ بالماكرو؛ |
| [GetExtendToAdjacentRange](./getextendtoadjacentrange/) | يشير إلى ما إذا كان يتم توسيع النطاقات عند نسخ النطاق إلى النطاق المجاور. |
| [SetExtendToAdjacentRange](./setextendtoadjacentrange/) | يشير إلى ما إذا كان يتم توسيع النطاقات عند نسخ النطاق إلى النطاق المجاور. |
| [GetCopyNames](./getcopynames/) | يشير إلى ما إذا كان يتم نسخ الأسماء. |
| [SetCopyNames](./setcopynames/) | يشير إلى ما إذا كان يتم نسخ الأسماء. |
| [GetCopyInvalidFormulasAsValues](./getcopyinvalidformulasasvalues/) | إذا كانت الصيغة غير صالحة للوجهة المستهدفة، يتم نسخ القيم فقط. |
| [SetCopyInvalidFormulasAsValues](./setcopyinvalidformulasasvalues/) | إذا كانت الصيغة غير صالحة للوجهة المستهدفة، يتم نسخ القيم فقط. |
| [GetColumnCharacterWidth](./getcolumncharacterwidth/) | يشير إلى ما إذا كان يتم نسخ عرض العمود بوحدة الأحرف. |
| [SetColumnCharacterWidth](./setcolumncharacterwidth/) | يشير إلى ما إذا كان يتم نسخ عرض العمود بوحدة الأحرف. |
| [GetReferToSheetWithSameName](./getrefertosheetwithsamename/) | في مايكروسوفت إكسل، عند نسخ الصيغ التي تشير إلى أوراق عمل أخرى أثناء نسخ ورقة عمل إلى أخرى، يجب أن تشير الصيغ المنسوخة إلى مصنف المصدر. ومع ذلك، في بعض الحالات قد يحتاج المستخدم إلى أن تشير الصيغ المنسوخة إلى أوراق عمل بنفس الاسم في نفس المصنف، مثل عندما يتم نسخ تلك الأوراق مسبقاً قبل عملية النسخ هذه، يجب أن تُحافظ على هذه الخاصية كصحيح. |
| [SetReferToSheetWithSameName](./setrefertosheetwithsamename/) | في مايكروسوفت إكسل، عند نسخ الصيغ التي تشير إلى أوراق عمل أخرى أثناء نسخ ورقة عمل إلى أخرى، يجب أن تشير الصيغ المنسوخة إلى مصنف المصدر. ومع ذلك، في بعض الحالات قد يحتاج المستخدم إلى أن تشير الصيغ المنسوخة إلى أوراق عمل بنفس الاسم في نفس المصنف، مثل عندما يتم نسخ تلك الأوراق مسبقاً قبل عملية النسخ هذه، يجب أن تُحافظ على هذه الخاصية كصحيح. |
| [GetReferToDestinationSheet](./getrefertodestinationsheet/) | عند نسخ النطاق في نفس الملف وكان المخطط يشير إلى ورقة المصدر، يعني False أن مصدر بيانات المخطط المنسوخ لن يتغير. يعني True أن مصدر بيانات المخطط المنسوخ يشير إلى ورقة الوجهة. |
| [SetReferToDestinationSheet](./setrefertodestinationsheet/) | عند نسخ النطاق في نفس الملف وكان المخطط يشير إلى ورقة المصدر، يعني False أن مصدر بيانات المخطط المنسوخ لن يتغير. يعني True أن مصدر بيانات المخطط المنسوخ يشير إلى ورقة الوجهة. |
| [GetUpdateInvalidReferencesToTargetSheet](./getupdateinvalidreferencestotargetsheet/) | يشير إلى ما إذا كان يجب الإشارة إلى ورقة العمل الهدف إذا لم يتم نسخ ورقة العمل المشار إليها. |
| [SetUpdateInvalidReferencesToTargetSheet](./setupdateinvalidreferencestotargetsheet/) | يشير إلى ما إذا كان يجب الإشارة إلى ورقة العمل الهدف إذا لم يتم نسخ ورقة العمل المشار إليها. |
