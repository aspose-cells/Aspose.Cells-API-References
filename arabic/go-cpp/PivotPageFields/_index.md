---
title: "PivotPageFields فئة"
linktitle: "PivotPageFields"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "PivotPageFields class. يغلف الكائن الذي يمثل pivotpagefields في Go."
type: docs
weight: 200
url: /ar/go-cpp/pivotpagefields/
---

## PivotPageFields class

يمثل عناصر صفحة المحور إذا كان مصدر بيانات جدول المحور هو نطاقات دمج. يمكن أن يحتوي على ما يصل إلى 4 عناصر فقط.

```go

type PivotPageFields struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewPivotPageFields](./newpivotpagefields/) | يمثل عناصر حقل صفحة المحور. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [AddPageField](./addpagefield/) | يضيف حقل صفحة. |
| [GetPageFieldCount](./getpagefieldcount/) | يحصل على عدد حقول الصفحة. |
| [AddIdentify](./addidentify/) | يضبط أي تسمية عنصر في كل حقل صفحة تُستخدم لتحديد نطاق البيانات. يجب أن يكون pageItemIndex.Length مساويًا لـ PageFieldCount، لذا يرجى إضافة حقل الصفحة أولاً. |
