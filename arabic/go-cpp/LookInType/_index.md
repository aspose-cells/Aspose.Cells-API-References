---
title: "LookInType تعداد"
linktitle: "LookInType"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "LookInType تعداد. يغلف الكائن الذي يمثل lookintype في Go."
type: docs
weight: 200
url: /ar/go-cpp/lookintype/
---

## LookInType Enum

يمثل نوع النظر داخل.

```go

type LookInType int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [Formulas](./formulas/) | يبحث عن الكائن المطلوب من الصيغة(<see cref=\"Cell.Formula\"/>) إذا كانت الخلية صيغة، وإلا يبحث من القيمة الأصلية للخلية (نفس <see cref=\"OriginalValues\"/>). |
| [Values](./values/) | يبحث عن الكائن من القيمة الأصلية للخلية(<see cref=\"Cell.Value\"/>) والقيمة المنسقة(<see cref=\"Cell.StringValue\"/>). |
| [ValuesExcludeFormulaCell](./valuesexcludeformulacell/) | يتجاهل الخلايا التي هي صيغ. بالنسبة لتلك الخلايا التي ليست صيغًا، يكون نفس <see cref=\"Values\"/>. |
| [Comments](./comments/) | يبحث عن الكائن من تعليق الخلية فقط. يتجاهل الخلايا التي لا تحتوي على تعليق. |
| [OnlyFormulas](./onlyformulas/) | يتجاهل الخلايا التي ليست صيغًا. بالنسبة لتلك الخلايا التي هي صيغ، يبحث عن الكائن المطلوب من الصيغة(<see cref=\"Cell.Formula\"/>). |
| [OriginalValues](./originalvalues/) | ابحث عن الكائن من القيمة الأصلية للخلية فقط. |
| [FormattedValues](./formattedvalues/) | ابحث عن الكائن من القيمة المنسقة للخلية(<see cref=\"Cell.StringValue\"/>) فقط. |
