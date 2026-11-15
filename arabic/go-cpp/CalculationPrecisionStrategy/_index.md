---
title: "CalculationPrecisionStrategy تعداد"
linktitle: "CalculationPrecisionStrategy"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "CalculationPrecisionStrategy تعداد. يغلف الكائن الذي يمثل calculationprecisionstrategy في Go."
type: docs
weight: 200
url: /ar/go-cpp/calculationprecisionstrategy/
---

## CalculationPrecisionStrategy Enum

يسرد استراتيجيات التعامل مع دقة الحساب. بسبب مشكلة الدقة في حسابات IEEE 754 ذات النقطة العائمة، قد لا تُحسب بعض الصيغ \"seemingly simple\" كما هو متوقع. مثل الصيغة \"=-0.45+0.43+0.02\"، عند حساب القيم باستخدام المشغل '+' مباشرةً، لا يكون الناتج صفراً. بالنسبة لهذا النوع من مشاكل الدقة، قد توفر بعض الاستراتيجيات الخاصة النتيجة المتوقعة.

```go

type CalculationPrecisionStrategy int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [None](./none/) | لا توجد استراتيجية مطبقة على الحساب. عند الحساب استخدم القيمة المزدوجة الأصلية كمعامل وأعد النتيجة مباشرة. الأكثر كفاءة للأداء ومطبق في معظم الحالات. |
| [Round](./round/) | يقوم بتقريب نتيجة الحساب وفقًا للأرقام ذات الدلالة. |
| [Decimal](./decimal/) | يستخدم العشري كمعاملات عندما يكون ذلك ممكنًا. الأكثر عدم كفاءة للأداء. |
