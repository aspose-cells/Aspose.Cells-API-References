---
title: "عدد CellValueFormatStrategy"
linktitle: "CellValueFormatStrategy"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "عدد CellValueFormatStrategy. يغلف الكائن الذي يمثل cellvalueformatstrategy في Go."
type: docs
weight: 200
url: /ar/go-cpp/cellvalueformatstrategy/
---

## CellValueFormatStrategy Enum

يحدد كيفية تطبيق النمط على قيمة الخلية.

```go

type CellValueFormatStrategy int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [None](./none/) | غير مُنسق. |
| [CellStyle](./cellstyle/) | مُنسق فقط باستخدام النمط الأصلي للخلية. |
| [DisplayStyle](./displaystyle/) | مُنسق باستخدام النمط المعروض للخلية. |
| [DisplayString](./displaystring/) | يحصل على السلسلة المعروضة في MS Excel. الفرق الرئيسي عن <see cref=\"DisplayStyle\"/> هو أن هذا الخيار يأخذ أيضًا في الاعتبار تأثير عرض العمود. إذا كان عرض العمود صغيرًا جدًا لعرض السلسلة المُنسقة بالكامل، قد يُظهر \"#\"، تمامًا كما يفعل MS Excel. |
