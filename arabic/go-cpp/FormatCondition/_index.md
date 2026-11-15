---
title: "فئة FormatCondition"
linktitle: "FormatCondition"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة FormatCondition. يغلف الكائن الذي يمثل formatcondition في Go."
type: docs
weight: 200
url: /ar/go-cpp/formatcondition/
---

## FormatCondition class

يمثل شرط تنسيق شرطي.

```go

type FormatCondition struct  {
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
| [GetFormula1_Bool_Bool](./getformula1_bool_bool/) | يحصل على القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| [GetFormula2_Bool_Bool](./getformula2_bool_bool/) | يحصل على القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| [GetFormula1_Bool_Bool_Int_Int](./getformula1_bool_bool_int_int/) | يحصل على القيمة أو التعبير لتنسيق الخلية الشرطي. |
| [GetFormula2_Bool_Bool_Int_Int](./getformula2_bool_bool_int_int/) | يحصل على القيمة أو التعبير لتنسيق الخلية الشرطي. |
| [SetFormulas](./setformulas/) | يضبط القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| [SetFormula1_String_Bool_Bool](./setformula1_string_bool_bool/) | يضبط القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| [SetFormula2_String_Bool_Bool](./setformula2_string_bool_bool/) | يضبط القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| [GetFormula1](./getformula1/) | يحصل ويضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [SetFormula1_String](./setformula1_string/) | يحصل ويضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [GetFormula1_Int_Int](./getformula1_int_int/) | يحصل على الصيغة لتنسيق الخلية الشرطي. |
| [GetFormula2](./getformula2/) | يحصل ويضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [SetFormula2_String](./setformula2_string/) | يحصل ويضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [GetFormula2_Int_Int](./getformula2_int_int/) | يحصل على الصيغة لتنسيق الخلية الشرطي. |
| [GetOperator](./getoperator/) | يحصل ويضبط نوع عامل التنسيق الشرطي. |
| [SetOperator](./setoperator/) | يحصل ويضبط نوع عامل التنسيق الشرطي. |
| [GetStopIfTrue](./getstopiftrue/) | صحيح، لا يمكن تطبيق أي قواعد ذات أولوية أقل فوق هذه القاعدة عندما تُقيم هذه القاعدة إلى true. ينطبق فقط على Excel 2007؛ |
| [SetStopIfTrue](./setstopiftrue/) | صحيح، لا يمكن تطبيق أي قواعد ذات أولوية أقل فوق هذه القاعدة عندما تُقيم هذه القاعدة إلى true. ينطبق فقط على Excel 2007؛ |
| [GetPriority](./getpriority/) | أولوية هذه القاعدة التنسيقية الشرطية. تُستخدم هذه القيمة لتحديد أي whichformat يجب تقييمه وعرضه. القيم الرقمية الأقل لها أولوية أعلى من thanhigher القيم الرقمية، حيث أن '1' هي أعلى أولوية. |
| [SetPriority](./setpriority/) | أولوية هذه القاعدة التنسيقية الشرطية. تُستخدم هذه القيمة لتحديد أي whichformat يجب تقييمه وعرضه. القيم الرقمية الأقل لها أولوية أعلى من thanhigher القيم الرقمية، حيث أن '1' هي أعلى أولوية. |
| [GetStyle](./getstyle/) | يحصل أو setts نمط نطاقات الخلايا المُنسقة شرطياً. |
| [SetStyle](./setstyle/) | يحصل أو setts نمط نطاقات الخلايا المُنسقة شرطياً. |
| [GetType](./gettype/) | يحصل ويضبط ما إذا كان نوع التنسيق الشرطي. |
| [SetType](./settype/) | يحصل ويضبط ما إذا كان نوع التنسيق الشرطي. |
| [GetIconSet](./geticonset/) | احصل على نسخة "IconSet" لتنسيق الشرطي. النسخة الافتراضية لها IconSetType هي TrafficLights31. صالحة فقط للنوع = IconSet. |
| [GetDataBar](./getdatabar/) | احصل على نسخة "DataBar" لتنسيق الشرطي. اللون الافتراضي للنسخة هو أزرق. صالحة فقط للنوع هو DataBar. |
| [GetColorScale](./getcolorscale/) | احصل على نسخة "ColorScale" لتنسيق الشرطي. النسخة الافتراضية هي "green-yellow-red" 3ColorScale. صالحة فقط للنوع = ColorScale. |
| [GetTop10](./gettop10/) | احصل على نسخة "Top10" لتنسيق الشرطي. القاعدة الافتراضية للنسخة تبرز الخلايا التي whosevalues تقع في أعلى 10 نطاقات. صالحة فقط للنوع هو Top10. |
| [GetAboveAverage](./getaboveaverage/) | احصل على نسخة "AboveAverage" لتنسيق الشرطي. القاعدة الافتراضية للنسخة تبرز الخلايا التي areabove المتوسط لجميع القيم في النطاق. صالحة فقط للنوع = AboveAverage. |
| [GetText](./gettext/) | قيمة النص في قاعدة تنسيق شرطي "text contains". صالحة فقط للنوع = containsText, notContainsText, beginsWith و endsWith. القيمة الافتراضية هي null. |
| [SetText](./settext/) | قيمة النص في قاعدة تنسيق شرطي "text contains". صالحة فقط للنوع = containsText, notContainsText, beginsWith و endsWith. القيمة الافتراضية هي null. |
| [GetTimePeriod](./gettimeperiod/) | الفترة الزمنية المطبقة في قاعدة تنسيق شرطي "date occurrin". صالحة فقط للنوع هو timePeriod. القيمة الافتراضية هي TimePeriodType.Today. |
| [SetTimePeriod](./settimeperiod/) | الفترة الزمنية المطبقة في قاعدة تنسيق شرطي "date occurrin". صالحة فقط للنوع هو timePeriod. القيمة الافتراضية هي TimePeriodType.Today. |
