---
title: "ErrorCheckType تعداد"
linktitle: "ErrorCheckType"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "ErrorCheckType تعداد. يغلف الكائن الذي يمثل errorchecktype في Go."
type: docs
weight: 200
url: /ar/go-cpp/errorchecktype/
---

## ErrorCheckType Enum

يمثل جميع أنواع فحص الأخطاء.

```go

type ErrorCheckType int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [EvaluationError](./evaluationerror/) | تجاهل الأخطاء عندما تحتوي الخلايا على صيغ تؤدي إلى خطأ. |
| [EmptyCellRef](./emptycellref/) | تجاهل الأخطاء عندما تشير الصيغ إلى خلايا فارغة. |
| [NumberStoredAsText](./numberstoredastext/) | تجاهل الأخطاء عندما تكون الأرقام مُنسقة كنص أو مسبوقة بعلامة اقتباس مفردة |
| [InconsistRange](./inconsistrange/) | تجاهل الأخطاء عندما تُغفل الصيغ خلايا معينة في منطقة. |
| [InconsistFormula](./inconsistformula/) | تجاهل الأخطاء عندما تختلف صيغة في منطقة من ورقة العمل الخاصة بك عن صيغ أخرى في نفس المنطقة. |
| [TwoDigitTextYear](./twodigittextyear/) | تجاهل الأخطاء عندما تحتوي الصيغ على خلايا مُنسقة كنص مع سنوات ممثلة برقمين. |
| [UnlockedFormula](./unlockedformula/) | تجاهل الأخطاء عندما تحتوي الخلايا غير المؤمنة على صيغ. |
| [TableDataValidation](./tabledatavalidation/) | تجاهل الأخطاء عندما لا يتوافق قيمة خلية في جدول مع قواعد التحقق من صحة البيانات المحددة. |
| [CalculatedColumn](./calculatedcolumn/) | تجاهل الأخطاء عندما تحتوي الخلايا على قيمة مختلفة عن صيغة العمود المحسوبة. |
