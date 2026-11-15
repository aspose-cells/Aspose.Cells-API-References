---
title: "عدد HyperlinkLoadMode"
linktitle: "HyperlinkLoadMode"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "عدد HyperlinkLoadMode. يغلف الكائن الذي يمثل hyperlinkloadmode في Go."
type: docs
weight: 200
url: /ar/go-cpp/hyperlinkloadmode/
---

## HyperlinkLoadMode Enum

يحدد كيفية معالجة الروابط التشعبية عند تحميل HTML.

```go

type HyperlinkLoadMode int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [Normal](./normal/) | يتم تحميل الرابط التشعبي الأول فقط في الخلية، وتُتجاهل الروابط التالية. |
| [AllowMultiple](./allowmultiple/) | يتم إضافة جميع الروابط التشعبية في الخلية إلى <see cref=\"Worksheet.Hyperlinks\"/>. لاحظ أن برنامج MS Excel يدعم رابطًا تشعبيًا واحدًا فقط لكل خلية، لذا قد ينتج عن هذا الخيار ملفات لا يستطيع Excel عرضها بالكامل. |
