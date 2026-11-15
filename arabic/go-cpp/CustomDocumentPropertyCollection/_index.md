---
title: "فئة CustomDocumentPropertyCollection"
linktitle: "CustomDocumentPropertyCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة CustomDocumentPropertyCollection. تغلف الكائن الذي يمثل customdocumentpropertycollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/customdocumentpropertycollection/
---

## CustomDocumentPropertyCollection class

مجموعة من خصائص المستند المخصصة.

```go

type CustomDocumentPropertyCollection struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewCustomDocumentPropertyCollection](./newcustomdocumentpropertycollection/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [Add_String_String](./add_string_string/) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات <b>PropertyType.String</b>. |
| [Add_String_Int](./add_string_int/) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات <b>PropertyType.Number</b>. |
| [Add_String_Date](./add_string_date/) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات <b>PropertyType.DateTime</b>. |
| [Add_String_Bool](./add_string_bool/) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات <b>PropertyType.Boolean</b>. |
| [Add_String_Double](./add_string_double/) | ينشئ خاصية مستند مخصصة جديدة من نوع البيانات <b>PropertyType.Float</b>. |
| [AddLinkToContent](./addlinktocontent/) | ينشئ خاصية مستند مخصصة جديدة ترتبط بالمحتوى. |
| [UpdateLinkedPropertyValue](./updatelinkedpropertyvalue/) | يحدّث قيم جميع الخصائص المخصصة المرتبطة بالمحتوى (استخدام قيمة الخلية للنطاق المرتبط لتحديث قيمة الخاصية المخصصة). |
| [UpdateLinkedRange](./updatelinkedrange/) | يحدّث جميع النطاقات المرتبطة بالخصائص المخصصة (استخدام قيمة الخاصية المخصصة لتحديث قيمة الخلية للنطاق المرتبط). |
| [Get_Int](./get_int/) | يرجع كائن DocumentProperty حسب الفهرس. |
| [Contains](./contains/) | يرجع true إذا كان هناك خاصية بالاسم المحدد موجودة في المجموعة. |
| [IndexOf](./indexof/) | يحصل على فهرس الخاصية حسب الاسم. |
| [Remove](./remove/) | يزيل خاصية بالاسم المحدد من المجموعة. |
| [RemoveAt](./removeat/) | يزيل خاصية في الفهرس المحدد. |
| [GetCount](./getcount/) | يحصل على عدد العناصر الموجودة في المثيل. |
