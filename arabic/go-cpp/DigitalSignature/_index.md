---
title: "فئة DigitalSignature"
linktitle: "DigitalSignature"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة DigitalSignature. تغلف الكائن الذي يمثل التوقيع الرقمي في Go."
type: docs
weight: 200
url: /ar/go-cpp/digitalsignature/
---

## DigitalSignature class

التوقيع في الملف.

```go

type DigitalSignature struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewDigitalSignature_Stream_String_String_Date](./newdigitalsignature_stream_string_string_date/) | منشئ DigitalSignature. |
| [NewDigitalSignature_String_String_String_Date](./newdigitalsignature_string_string_string_date/) | منشئ DigitalSignature. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetComments](./getcomments/) | الغرض من التوقيع. |
| [SetComments](./setcomments/) | الغرض من التوقيع. |
| [GetSignTime](./getsigntime/) | الوقت الذي تم فيه توقيع المستند. |
| [SetSignTime](./setsigntime/) | الوقت الذي تم فيه توقيع المستند. |
| [GetId](./getid/) | يحدد GUID يمكن الإشارة إليه عبر GUID لسطر التوقيع المخزن في محتوى المستند. القيمة الافتراضية هي Empty (جميع الأصفار) Guid. |
| [SetId](./setid/) | يحدد GUID يمكن الإشارة إليه عبر GUID لسطر التوقيع المخزن في محتوى المستند. القيمة الافتراضية هي Empty (جميع الأصفار) Guid. |
| [GetText](./gettext/) | يحدد نص التوقيع الفعلي في التوقيع الرقمي. القيمة الافتراضية هي Empty. |
| [SetText](./settext/) | يحدد نص التوقيع الفعلي في التوقيع الرقمي. القيمة الافتراضية هي Empty. |
| [GetImage](./getimage/) | يحدد صورة للتوقيع الرقمي. القيمة الافتراضية هي null. |
| [SetImage](./setimage/) | يحدد صورة للتوقيع الرقمي. القيمة الافتراضية هي null. |
| [GetProviderId](./getproviderid/) | يحدد معرف الفئة لمزود التوقيع. القيمة الافتراضية هي Empty (جميع الأصفار) Guid. |
| [SetProviderId](./setproviderid/) | يحدد معرف الفئة لمزود التوقيع. القيمة الافتراضية هي Empty (جميع الأصفار) Guid. |
| [IsValid](./isvalid/) | إذا كانت هذه التوقيع الرقمي صالحًا ولم يتم العبث بالمستند، فستكون هذه القيمة صحيحة. |
| [GetXAdESType](./getxadestype/) | نوع XAdES. القيمة الافتراضية هي لا شيء (XAdES غير مفعل). |
| [SetXAdESType](./setxadestype/) | نوع XAdES. القيمة الافتراضية هي لا شيء (XAdES غير مفعل). |
