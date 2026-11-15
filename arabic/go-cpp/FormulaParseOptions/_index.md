---
title: "فئة FormulaParseOptions"
linktitle: "FormulaParseOptions"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة FormulaParseOptions. تغلف الكائن الذي يمثل formulaparseoptions في Go."
type: docs
weight: 200
url: /ar/go-cpp/formulaparseoptions/
---

## FormulaParseOptions class

يمثل الخيارات عند تحليل الصيغة.

```go

type FormulaParseOptions struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewFormulaParseOptions](./newformulaparseoptions/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetLocaleDependent](./getlocaledependent/) | ما إذا كانت الصيغة مهيأة وفق الإعدادات المحلية. القيمة الافتراضية هي false. |
| [SetLocaleDependent](./setlocaledependent/) | ما إذا كانت الصيغة مهيأة وفق الإعدادات المحلية. القيمة الافتراضية هي false. |
| [GetR1C1Style](./getr1c1style/) | ما إذا كانت الصيغة بنمط الإشارة R1C1. القيمة الافتراضية هي false. |
| [SetR1C1Style](./setr1c1style/) | ما إذا كانت الصيغة بنمط الإشارة R1C1. القيمة الافتراضية هي false. |
| [GetCheckAddIn](./getcheckaddin/) | ما إذا يتم فحص الإضافات في الروابط الخارجية الموجودة لدفتر العمل الحالي للوظيفة المعرفة من قبل المستخدم دون رابط خارجي. القيمة الافتراضية هي true (إذا تطابقت الوظيفة المعرفة من قبل المستخدم مع إحدى الإضافات في الروابط الخارجية الموجودة، فسيتم اعتبارها الإضافة). |
| [SetCheckAddIn](./setcheckaddin/) | ما إذا يتم فحص الإضافات في الروابط الخارجية الموجودة لدفتر العمل الحالي للوظيفة المعرفة من قبل المستخدم دون رابط خارجي. القيمة الافتراضية هي true (إذا تطابقت الوظيفة المعرفة من قبل المستخدم مع إحدى الإضافات في الروابط الخارجية الموجودة، فسيتم اعتبارها الإضافة). |
| [GetParse](./getparse/) | ما إذا يتم تحليل الصيغة المعطاة. القيمة الافتراضية هي true. إذا كانت false، فستبقى سلسلة الصيغة المعطاة كما هي للخلية حتى يقوم المستخدم باستدعاء طرق أخرى لتحليلها أو عندما تكون بيانات الصيغة المحللة مطلوبة من قبل عمليات أخرى مثل حساب الصيغ. |
| [SetParse](./setparse/) | ما إذا يتم تحليل الصيغة المعطاة. القيمة الافتراضية هي true. إذا كانت false، فستبقى سلسلة الصيغة المعطاة كما هي للخلية حتى يقوم المستخدم باستدعاء طرق أخرى لتحليلها أو عندما تكون بيانات الصيغة المحللة مطلوبة من قبل عمليات أخرى مثل حساب الصيغ. |
| [GetCustomFunctionDefinition](./getcustomfunctiondefinition/) | تعريف لتحليل الدوال المخصصة. |
| [SetCustomFunctionDefinition](./setcustomfunctiondefinition/) | تعريف لتحليل الدوال المخصصة. |
