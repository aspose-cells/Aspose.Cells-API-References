---
title: "SignatureLine فئة"
linktitle: "SignatureLine"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "SignatureLine فئة. يغلف الكائن الذي يمثل signatureline في Go."
type: docs
weight: 200
url: /ar/go-cpp/signatureline/
---

## SignatureLine class

يمثل خط التوقيع.

```go

type SignatureLine struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewSignatureLine](./newsignatureline/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetId](./getid/) | يحصل أو يعيّن المعرف لهذا سطر التوقيع. |
| [SetId](./setid/) | يحصل أو يعيّن المعرف لهذا سطر التوقيع. |
| [GetProviderId](./getproviderid/) | يحصل أو يعيّن معرف موفر التوقيع. |
| [SetProviderId](./setproviderid/) | يحصل أو يعيّن معرف موفر التوقيع. |
| [GetSigner](./getsigner/) | يحصل أو يعيّن المُوقّع. |
| [SetSigner](./setsigner/) | يحصل أو يعيّن المُوقّع. |
| [GetTitle](./gettitle/) | يحصل أو يعيّن عنوان المغني. |
| [SetTitle](./settitle/) | يحصل أو يعيّن عنوان المغني. |
| [GetEmail](./getemail/) | يحصل أو يعيّن البريد الإلكتروني للمغني. |
| [SetEmail](./setemail/) | يحصل أو يعيّن البريد الإلكتروني للمغني. |
| [IsLine](./isline/) | يشير ما إذا كان سطر توقيع. |
| [SetIsLine](./setisline/) | يشير ما إذا كان سطر توقيع. |
| [GetAllowComments](./getallowcomments/) | يشير ما إذا كان يمكن إرفاق التعليقات. |
| [SetAllowComments](./setallowcomments/) | يشير ما إذا كان يمكن إرفاق التعليقات. |
| [GetShowSignedDate](./getshowsigneddate/) | يشير ما إذا كان يُظهر تاريخ التوقيع. |
| [SetShowSignedDate](./setshowsigneddate/) | يشير ما إذا كان يُظهر تاريخ التوقيع. |
| [GetInstructions](./getinstructions/) | يحصل أو يعيّن النص المعروض للمستخدم عند توقيع. |
| [SetInstructions](./setinstructions/) | يحصل أو يعيّن النص المعروض للمستخدم عند توقيع. |
| [GetSignatureLineType](./getsignaturelinetype/) | يحصل أو يعيّن نوع التوقيع. Default - عندما يتم تعيين القيمة الافتراضية، تكون قيمة ProviderId المقابلة ثابتة إلى {0000000000-0000-0000-0000-0000000000}. Stamp - عندما تكون القيمة Stamp، تكون قيمة ProviderId المقابلة عادةً {000CD6A4-0000-0000-C000-000000000046}. Custom - عندما تكون القيمة Custom، عادةً ما تحتاج قيمة ProviderId المقابلة إلى أن يحددها المستخدم. يجب الحصول عليها من الوثائق المرفقة مع الموفر. |
| [SetSignatureLineType](./setsignaturelinetype/) | يحصل أو يعيّن نوع التوقيع. Default - عندما يتم تعيين القيمة الافتراضية، تكون قيمة ProviderId المقابلة ثابتة إلى {0000000000-0000-0000-0000-0000000000}. Stamp - عندما تكون القيمة Stamp، تكون قيمة ProviderId المقابلة عادةً {000CD6A4-0000-0000-C000-000000000046}. Custom - عندما تكون القيمة Custom، عادةً ما تحتاج قيمة ProviderId المقابلة إلى أن يحددها المستخدم. يجب الحصول عليها من الوثائق المرفقة مع الموفر. |
