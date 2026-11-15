---
title: "فئة ConditionalFormattingValue"
linktitle: "ConditionalFormattingValue"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ConditionalFormattingValue. تغلف الكائن الذي يمثل conditionalformattingvalue في Go."
type: docs
weight: 200
url: /ar/go-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

يصف قيم نقاط الاستيفاء في مقياس متدرج أو شريط بيانات أو مجموعة أيقونات.

```go

type ConditionalFormattingValue struct  {
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
| [GetValue](./getvalue/) | احصل على أو اضبط قيمة كائن قيمة التنسيق الشرطي هذا. يجب استخدامه بالاشتراك مع Type. |
| [SetValue](./setvalue/) | احصل على أو اضبط قيمة كائن قيمة التنسيق الشرطي هذا. يجب استخدامه بالاشتراك مع Type. |
| [GetType](./gettype/) | احصل على أو اضبط نوع كائن قيمة التنسيق الشرطي هذا. ضبط النوع إلى FormatConditionValueType.Min أو FormatConditionValueType.Max سيؤدي تلقائيًا إلى تعيين "Value" إلى null. |
| [SetType](./settype/) | احصل على أو اضبط نوع كائن قيمة التنسيق الشرطي هذا. ضبط النوع إلى FormatConditionValueType.Min أو FormatConditionValueType.Max سيؤدي تلقائيًا إلى تعيين "Value" إلى null. |
| [IsGTE](./isgte/) | احصل على أو اضبط علامة أكبر من أو يساوي. استخدم فقط لمجموعات الأيقونات، يحدد ما إذا كانت قيمة العتبة هذه تستخدم عامل أكبر من أو يساوي. 'false' تشير إلى أن 'greater than' يُستخدم بدلاً من 'greater than or equal to'. القيمة الافتراضية هي true. |
| [SetIsGTE](./setisgte/) | احصل على أو اضبط علامة أكبر من أو يساوي. استخدم فقط لمجموعات الأيقونات، يحدد ما إذا كانت قيمة العتبة هذه تستخدم عامل أكبر من أو يساوي. 'false' تشير إلى أن 'greater than' يُستخدم بدلاً من 'greater than or equal to'. القيمة الافتراضية هي true. |
