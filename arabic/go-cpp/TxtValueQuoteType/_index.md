---
title: "تعداد TxtValueQuoteType"
linktitle: "TxtValueQuoteType"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "تعداد TxtValueQuoteType. يغلف الكائن الذي يمثل txtvaluequotetype في Go."
type: docs
weight: 200
url: /ar/go-cpp/txtvaluequotetype/
---

## TxtValueQuoteType Enum

يحدد نوع استخدام علامات الاقتباس للقيم في ملفات النص.

```go

type TxtValueQuoteType int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [Normal](./normal/) | جميع القيم التي تحتوي على أحرف خاصة مثل علامة الاقتباس أو حرف الفاصل سيتم اقتباسها. نفس سلوك برنامج ms excel عند تصدير ملف نصي. |
| [Always](./always/) | جميع القيم سيتم اقتباسها دائمًا. |
| [Minimum](./minimum/) | اقتبس القيم فقط عندما يكون ذلك ضروريًا. على سبيل المثال، إذا احتوت قيمة ما علامة اقتباس ولكن علامة الاقتباس ليست في بداية هذه القيمة، فلن يتم اقتباس هذه القيمة. |
| [Never](./never/) | لن يتم اقتباس جميع القيم. قد لا يتم قراءة ملف النص المُصدَّر بهذا النوع بشكل صحيح بسبب عدم وجود علامات الاقتباس اللازمة. |
