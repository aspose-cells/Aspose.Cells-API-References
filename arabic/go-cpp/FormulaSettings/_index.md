---
title: "فئة FormulaSettings"
linktitle: "FormulaSettings"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة FormulaSettings. يغلف الكائن الذي يمثل formulasettings في Go."
type: docs
weight: 200
url: /ar/go-cpp/formulasettings/
---

## FormulaSettings class

إعدادات الصيغ والحساب.

```go

type FormulaSettings struct  {
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
| [GetCalculateOnOpen](./getcalculateonopen/) | يشير إلى ما إذا كان التطبيق مطلوبًا لإجراء حساب كامل عند فتح دفتر العمل. |
| [SetCalculateOnOpen](./setcalculateonopen/) | يشير إلى ما إذا كان التطبيق مطلوبًا لإجراء حساب كامل عند فتح دفتر العمل. |
| [GetCalculateOnSave](./getcalculateonsave/) | يشير إلى ما إذا كان يجب إعادة حساب دفتر العمل قبل حفظ المستند، عندما يكون في وضع الحساب اليدوي. |
| [SetCalculateOnSave](./setcalculateonsave/) | يشير إلى ما إذا كان يجب إعادة حساب دفتر العمل قبل حفظ المستند، عندما يكون في وضع الحساب اليدوي. |
| [GetForceFullCalculation](./getforcefullcalculation/) | يشير إلى ما إذا كان يحسب جميع الصيغ في كل مرة يتم فيها تشغيل حساب. |
| [SetForceFullCalculation](./setforcefullcalculation/) | يشير إلى ما إذا كان يحسب جميع الصيغ في كل مرة يتم فيها تشغيل حساب. |
| [GetCalculationMode](./getcalculationmode/) | يحصل أو يضبط وضع حساب دفتر العمل في MS Excel. |
| [SetCalculationMode](./setcalculationmode/) | يحصل أو يضبط وضع حساب دفتر العمل في MS Excel. |
| [GetCalculationId](./getcalculationid/) | يحدد إصدار محرك الحساب المستخدم لحساب القيم في دفتر العمل. |
| [SetCalculationId](./setcalculationid/) | يحدد إصدار محرك الحساب المستخدم لحساب القيم في دفتر العمل. |
| [GetEnableIterativeCalculation](./getenableiterativecalculation/) | يشير إلى ما إذا كان يجب تمكين الحساب التكراري لحل المراجع الدائرية. |
| [SetEnableIterativeCalculation](./setenableiterativecalculation/) | يشير إلى ما إذا كان يجب تمكين الحساب التكراري لحل المراجع الدائرية. |
| [GetMaxIteration](./getmaxiteration/) | الحد الأقصى للتكرارات لحل مرجع دائري. |
| [SetMaxIteration](./setmaxiteration/) | الحد الأقصى للتكرارات لحل مرجع دائري. |
| [GetMaxChange](./getmaxchange/) | الحد الأقصى للتغيير لحل مرجع دائري. |
| [SetMaxChange](./setmaxchange/) | الحد الأقصى للتغيير لحل مرجع دائري. |
| [GetPrecisionAsDisplayed](./getprecisionasdisplayed/) | يشير إلى ما إذا كان يجب ضبط دقة النتيجة المحسوبة كما تُعرض أثناء حساب الصيغ. |
| [SetPrecisionAsDisplayed](./setprecisionasdisplayed/) | يشير إلى ما إذا كان يجب ضبط دقة النتيجة المحسوبة كما تُعرض أثناء حساب الصيغ. |
| [GetEnableCalculationChain](./getenablecalculationchain/) | يشير إلى ما إذا كان يجب تمكين سلسلة الحساب للصيغ. القيمة الافتراضية هي false. |
| [SetEnableCalculationChain](./setenablecalculationchain/) | يشير إلى ما إذا كان يجب تمكين سلسلة الحساب للصيغ. القيمة الافتراضية هي false. |
| [GetPreservePaddingSpaces](./getpreservepaddingspaces/) | يشير إلى ما إذا كان يجب الحفاظ على تلك الفراغات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false. |
| [SetPreservePaddingSpaces](./setpreservepaddingspaces/) | يشير إلى ما إذا كان يجب الحفاظ على تلك الفراغات وفواصل الأسطر التي تُضاف بين رموز الصيغة أثناء الحصول على الصيغ وتعيينها. القيمة الافتراضية هي false. |
