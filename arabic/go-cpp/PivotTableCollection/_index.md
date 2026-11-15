---
title: "فئة PivotTableCollection"
linktitle: "PivotTableCollection"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PivotTableCollection. تغلف الكائن الذي يمثل PivotTableCollection في Go."
type: docs
weight: 200
url: /ar/go-cpp/pivottablecollection/
---

## PivotTableCollection class

يمثل مجموعة جميع كائنات PivotTable في ورقة العمل المحددة.

```go

type PivotTableCollection struct  {
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
| [Dispose](./dispose/) | يؤدي مهامًا محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
| [Add_String_Int_Int](./add_string_int_int/) | يضيف PivotTable جديدًا في الصف والعمود المحددين في ورقة العمل مع الخيارات الافتراضية. |
| [Add_String_Int_Int_String_Bool_Bool](./add_string_int_int_string_bool_bool/) | يضيف PivotTable جديدًا بتخطيط ونمط Excel 97-2003 القديم. |
| [Add_String_String_String_Bool_Bool](./add_string_string_string_bool_bool/) | يضيف PivotTable جديدًا. |
| [Add_PivotTable_String_String](./add_pivottable_string_string/) | يضيف PivotTable جديدًا بناءً على PivotTable آخر. |
| [Add_PivotTable_Int_Int_String](./add_pivottable_int_int_string/) | يضيف PivotTable جديدًا بناءً على PivotTable آخر. |
| [Add_stringArray_Bool_PivotPageFields_String_String](./add_stringarray_bool_pivotpagefields_string_string/) | يضيف كائن PivotTable جديد إلى المجموعة مع نطاقات تجميع متعددة كمصدر للبيانات. |
| [Add_stringArray_Bool_PivotPageFields_Int_Int_String](./add_stringarray_bool_pivotpagefields_int_int_string/) | يضيف كائن PivotTable جديد إلى المجموعة مع نطاقات تجميع متعددة كمصدر للبيانات. |
| [Get_Int](./get_int/) | يحصل على تقرير PivotTable حسب الفهرس. |
| [Get_String](./get_string/) | يحصل على تقرير PivotTable حسب اسم الـ PivotTable. |
| [Get_Int_Int](./get_int_int/) | يحصل على تقرير PivotTable حسب موقع الـ PivotTable. |
| [Clear](./clear/) | يمسح جميع جداول PivotTable. |
| [Remove_PivotTable](./remove_pivottable/) | يحذف PivotTable المحدد ويحذف بيانات PivotTable. |
| [Remove_PivotTable_Bool](./remove_pivottable_bool/) | يحذف PivotTable المحدد. |
| [RemoveAt_Int](./removeat_int/) | يحذف PivotTable في الفهرس المحدد ويحذف بيانات PivotTable. |
| [RemoveAt_Int_Bool](./removeat_int_bool/) | يحذف PivotTable في الفهرس المحدد. |
| [GetCount](./getcount/) | يحصل على عدد العناصر الموجودة في المثيل. |
