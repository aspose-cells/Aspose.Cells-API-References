---
title: "فئة WebExtension"
linktitle: "WebExtension"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة WebExtension. تغلف الكائن الذي يمثل webextension في Go."
type: docs
weight: 200
url: /ar/go-cpp/webextension/
---

## WebExtension class

يمثل نسخة من Office Add-in.

```go

type WebExtension struct  {
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
| [GetId](./getid/) | يحصل أو يعيّن المعرف الفريد لنسخة Office Add-in في المستند الحالي. |
| [SetId](./setid/) | يحصل أو يعيّن المعرف الفريد لنسخة Office Add-in في المستند الحالي. |
| [IsFrozen](./isfrozen/) | يشير إلى ما إذا كان المستخدم يمكنه التفاعل مع Office Add-in أم لا. |
| [SetIsFrozen](./setisfrozen/) | يشير إلى ما إذا كان المستخدم يمكنه التفاعل مع Office Add-in أم لا. |
| [GetReference](./getreference/) | احصل على المرجع الأساسي لـ Office Add-in. |
| [GetAlterReferences](./getalterreferences/) | يحصل على قائمة بالمراجع البديلة. |
| [GetProperties](./getproperties/) | يحصل على جميع خصائص web extension. |
| [GetBindings](./getbindings/) | يحصل على جميع علاقات الربط بين Office Add-in والبيانات في المستند. |
