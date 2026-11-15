---
title: "فئة LowCodeSaveOptions"
linktitle: "LowCodeSaveOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة LowCodeSaveOptions. تغلف الكائن الذي يمثل lowcodesaveoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/lowcodesaveoptions/
---

## LowCodeSaveOptions class

خيارات لحفظ النتائج المولدة بطريقة منخفضة الكود.

```go

type LowCodeSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewLowCodeSaveOptions](./newlowcodesaveoptions/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetOutputFile](./getoutputfile/) | يحصل ويحدد الملف (مع المسار إذا لزم الأمر) لحفظ البيانات المُولدة. عند تعيين هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل OutputStream. |
| [SetOutputFile](./setoutputfile/) | يحصل ويحدد الملف (مع المسار إذا لزم الأمر) لحفظ البيانات المُولدة. عند تعيين هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل OutputStream. |
| [GetOutputStream](./getoutputstream/) | يحصل ويحدد الـ Stream لكتابة البيانات المُولدة إليه. عند تعيين هذه الخاصية بقيمة غير null، سيتم تجاهل OutputFile. |
| [SetOutputStream](./setoutputstream/) | يحصل ويحدد الـ Stream لكتابة البيانات المُولدة إليه. عند تعيين هذه الخاصية بقيمة غير null، سيتم تجاهل OutputFile. |
| [GetSaveFormat](./getsaveformat/) | يحصل على ويضبط تنسيق الحفظ للإخراج. عادةً، بالنسبة للعمليات المحددة بطريقة منخفضة الشيفرة، يُسمح فقط ببعض التنسيقات المحددة. يرجى تحديد التنسيق الصحيح للعملية المقابلة، وإلا قد يحدث نتيجة غير متوقعة أو حتى استثناء. |
| [SetSaveFormat](./setsaveformat/) | يحصل على ويضبط تنسيق الحفظ للإخراج. عادةً، بالنسبة للعمليات المحددة بطريقة منخفضة الشيفرة، يُسمح فقط ببعض التنسيقات المحددة. يرجى تحديد التنسيق الصحيح للعملية المقابلة، وإلا قد يحدث نتيجة غير متوقعة أو حتى استثناء. |
