---
title: "فئة LowCodePdfSaveOptions"
linktitle: "LowCodePdfSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة LowCodePdfSaveOptions. تغلف الكائن الذي يمثل lowcodepdfsaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/lowcodepdfsaveoptions/
---

## LowCodePdfSaveOptions class

خيارات لحفظ pdf بطريقة منخفضة الكود.

```go

type LowCodePdfSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewLowCodePdfSaveOptions](./newlowcodepdfsaveoptions/) | البناء الافتراضي. |
| [NewLowCodePdfSaveOptions_LowCodeSaveOptions](./newlowcodepdfsaveoptions_lowcodesaveoptions/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetSaveFormat](./getsaveformat/) | تنسيق الحفظ للإخراج. لتحويل إلى pdf، يمكن أن يكون فقط SaveFormat.Pdf. |
| [SetSaveFormat](./setsaveformat/) | تنسيق الحفظ للإخراج. لتحويل إلى pdf، يمكن أن يكون فقط SaveFormat.Pdf. |
| [GetPdfOptions](./getpdfoptions/) | الخيارات لحفظ ملف Pdf. |
| [SetPdfOptions](./setpdfoptions/) | الخيارات لحفظ ملف Pdf. |
| [GetOutputFile](./getoutputfile/) | يحصل ويحدد الملف (مع المسار إذا لزم الأمر) لحفظ البيانات المُولدة. عند تعيين هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل OutputStream. |
| [SetOutputFile](./setoutputfile/) | يحصل ويحدد الملف (مع المسار إذا لزم الأمر) لحفظ البيانات المُولدة. عند تعيين هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل OutputStream. |
| [GetOutputStream](./getoutputstream/) | يحصل ويحدد الـ Stream لكتابة البيانات المُولدة إليه. عند تعيين هذه الخاصية بقيمة غير null، سيتم تجاهل OutputFile. |
| [SetOutputStream](./setoutputstream/) | يحصل ويحدد الـ Stream لكتابة البيانات المُولدة إليه. عند تعيين هذه الخاصية بقيمة غير null، سيتم تجاهل OutputFile. |
