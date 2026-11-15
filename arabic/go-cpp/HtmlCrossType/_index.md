---
title: "HtmlCrossType تعداد"
linktitle: "HtmlCrossType"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "HtmlCrossType تعداد. يغلف الكائن الذي يمثل htmlcrosstype في Go."
type: docs
weight: 200
url: /ar/go-cpp/htmlcrosstype/
---

## HtmlCrossType Enum

يمثل خمسة أنواع من سلاسل html المتقاطعة.

```go

type HtmlCrossType int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [Default](./default/) | يعرض مثل MS Excel، يعتمد على الخلية التالية. إذا كانت الخلية التالية فارغة، سيتقاطع النص، أو سيُقص. |
| [MSExport](./msexport/) | اعرض السلسلة مثل MS Excel عند تصدير html. |
| [Cross](./cross/) | عرض سلسلة HTML المتقاطعة، سيكون هذا الأداء لإنشاء ملفات HTML الكبيرة أسرع بأكثر من عشرة أضعاف مقارنةً بتعيين القيمة إلى Default أو FitToCell. |
| [CrossHideRight](./crosshideright/) | عرض سلسلة HTML المتقاطعة وإخفاء السلسلة اليمنى عندما تتداخل النصوص. |
| [FitToCell](./fittocell/) | عرض السلسلة فقط ضمن عرض الخلية. |
