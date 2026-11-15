---
title: "ReConnectionMethodType Enum"
linktitle: "ReConnectionMethodType"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "ReConnectionMethodType enum. تغلف الكائن الذي يمثل reconnectionmethodtype في Go."
type: docs
weight: 200
url: /ar/go-cpp/reconnectionmethodtype/
---

## ReConnectionMethodType Enum

يحدد ما يجب أن تفعله تطبيقات الجداول عندما يفشل الاتصال.

```go

type ReConnectionMethodType int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [Required](./required/) | عند التحديث استخدم معلومات الاتصال الحالية وإذا تبين أنها غير صالحة فاحصل على معلومات اتصال محدثة، إذا كانت متوفرة من ملف الاتصال الخارجي. |
| [Always](./always/) | في كل تحديث احصل على معلومات الاتصال المحدثة من ملف الاتصال الخارجي، إذا كان متوفرًا، واستخدمها بدلاً من معلومات الاتصال الحالية. في هذه الحالة سيفشل تحديث البيانات إذا كان ملف الاتصال الخارجي غير متوفر. |
| [Never](./never/) | لا تحصل أبدًا على معلومات الاتصال المحدثة من ملف الاتصال الخارجي حتى إذا كان متوفرًا وحتى إذا كانت معلومات الاتصال الحالية غير صالحة |
