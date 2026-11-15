---
title: "فئة AbstractLowCodeSaveOptionsProvider"
linktitle: "AbstractLowCodeSaveOptionsProvider"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "AbstractLowCodeSaveOptionsProvider class. تغلف الكائن الذي يمثل abstractlowcodesaveoptionsprovider في Go."
type: docs
weight: 200
url: /ar/go-cpp/abstractlowcodesaveoptionsprovider/
---

## AbstractLowCodeSaveOptionsProvider class

تنفيذ لتوفير خيارات حفظ متعددة للعمليات التي تتطلب مخرجات متعددة. على سبيل المثال، ميزة <see cref=\"SpreadsheetSplitter\"/> تتطلب وجهات متعددة لحفظ الملفات المقسمة.

```go

type AbstractLowCodeSaveOptionsProvider struct  {
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
| [GetSaveOptions](./getsaveoptions/) | يحصل على خيارات الحفظ التي يتم منها الحصول على إعدادات الإخراج للجزء المقسم حالياً. إرجاع null يعني تخطي الجزء المحدد. |
| [Finish](./finish/) | يطلق الموارد بعد معالجة الجزء المقسم حالياً. |
