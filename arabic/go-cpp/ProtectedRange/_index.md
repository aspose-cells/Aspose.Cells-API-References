---
title: "فئة ProtectedRange"
linktitle: "ProtectedRange"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة ProtectedRange. تغلف الكائن الذي يمثل protectedrange في Go."
type: docs
weight: 200
url: /ar/go-cpp/protectedrange/
---

## ProtectedRange class

نطاق محدد يُسمح بتحريره عندما يكون حماية الورقة مفعلة.

```go

type ProtectedRange struct  {
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
| [GetName](./getname/) | يحصل على عنوان النطاق. يُستخدم هذا كواصف، وليس كتعريف نطاق مسمى. |
| [SetName](./setname/) | يحصل على عنوان النطاق. يُستخدم هذا كواصف، وليس كتعريف نطاق مسمى. |
| [GetCellArea](./getcellarea/) | يحصل على كائن CellArea الذي يمثل مساحة الخلية التي سيتم حمايتها. |
| [GetAreas](./getareas/) | يحصل على جميع المناطق المشار إليها. |
| [AddArea](./addarea/) | يضيف منطقة مشار إليها إلى هذا. |
| [IsProtectedWithPassword](./isprotectedwithpassword/) | يشير إلى ما إذا كانت ورقة العمل محمية بكلمة مرور. |
| [GetPassword](./getpassword/) | يمثل كلمة المرور لحماية النطاق. |
| [SetPassword](./setpassword/) | يمثل كلمة المرور لحماية النطاق. |
| [GetSecurityDescriptor](./getsecuritydescriptor/) | يحدد الوصف الأمني حسابات المستخدمين الذين يمكنهم تعديل هذا النطاق دون تقديم كلمة مرور للوصول إلى النطاق. |
| [SetSecurityDescriptor](./setsecuritydescriptor/) | يحدد الوصف الأمني حسابات المستخدمين الذين يمكنهم تعديل هذا النطاق دون تقديم كلمة مرور للوصول إلى النطاق. |
