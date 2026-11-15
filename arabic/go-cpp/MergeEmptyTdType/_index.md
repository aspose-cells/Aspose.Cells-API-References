---
title: "عدد MergeEmptyTdType Enum"
linktitle: "MergeEmptyTdType"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "عدد MergeEmptyTdType enum. يغلف الكائن الذي يمثل mergeemptytdtype في Go."
type: docs
weight: 200
url: /ar/go-cpp/mergeemptytdtype/
---

## MergeEmptyTdType Enum

يمثل نوع الدمج لعنصر TD فارغ عند تصدير ملف إلى HTML.

```go

type MergeEmptyTdType int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [Default](./default/) | عرض مشابه لـ MS Excel. |
| [None](./none/) | لن يتم دمج عناصر TD الفارغة عند تصدير الملف إلى HTML. سيؤدي ذلك إلى إنشاء ملف HTML أكبر بكثير. |
| [MergeForcely](./mergeforcely/) | دمج عنصر TD الفارغ إجباريًا عند تصدير الملف إلى HTML. سيقل حجم ملف HTML بشكل كبير بعد ضبط القيمة على true. إذا كنت ترغب في استيراد ملف HTML إلى Excel أو تصدير خطوط شبكة مثالية عند حفظ الملف كـ HTML، يرجى الحفاظ على القيمة الافتراضية. |
