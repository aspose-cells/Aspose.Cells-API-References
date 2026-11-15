---
title: "DataSorter فئة"
linktitle: "DataSorter"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "DataSorter class. يغلف الكائن الذي يمثل datasorter في Go."
type: docs
weight: 200
url: /ar/go-cpp/datasorter/
---

## DataSorter class

وصف موجز لـ DataSorter.

```go

type DataSorter struct  {
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
| [GetKeys](./getkeys/) | يحصل على قائمة المفاتيح لمُرتّب البيانات. |
| [Clear](./clear/) | امسح جميع الإعدادات. |
| [GetHasHeaders](./gethasheaders/) | يمثل ما إذا كان النطاق يحتوي على رؤوس. |
| [SetHasHeaders](./sethasheaders/) | يمثل ما إذا كان النطاق يحتوي على رؤوس. |
| [AddKey_Int_SortOrder](./addkey_int_sortorder/) | يضيف فهرس العمود المرتب وترتيب الفرز. |
| [AddKey_Int_SortOrder_String](./addkey_int_sortorder_string/) | يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة. |
| [AddColorKey](./addcolorkey/) | يضيف مفتاح فرز اللون. |
| [AddKey_Int_SortOnType_SortOrder_Object](./addkey_int_sortontype_sortorder_object/) | يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة. |
| [AddKey_Int_SortOrder_stringArray](./addkey_int_sortorder_stringarray/) | يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة. |
| [GetKey1](./getkey1/) | يمثل فهرس العمود المرتب الأول (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [SetKey1](./setkey1/) | يمثل فهرس العمود المرتب الأول (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [GetOrder1](./getorder1/) | يمثل ترتيب الفرز للمفتاح الأول. |
| [SetOrder1](./setorder1/) | يمثل ترتيب الفرز للمفتاح الأول. |
| [GetKey2](./getkey2/) | يمثل فهرس العمود المرتب الثاني (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [SetKey2](./setkey2/) | يمثل فهرس العمود المرتب الثاني (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [GetOrder2](./getorder2/) | يمثل ترتيب الفرز للمفتاح الثاني. |
| [SetOrder2](./setorder2/) | يمثل ترتيب الفرز للمفتاح الثاني. |
| [GetKey3](./getkey3/) | يمثل فهرس العمود المرتب الثالث (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [SetKey3](./setkey3/) | يمثل فهرس العمود المرتب الثالث (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [GetOrder3](./getorder3/) | يمثل ترتيب الفرز للمفتاح الثالث. |
| [SetOrder3](./setorder3/) | يمثل ترتيب الفرز للمفتاح الثالث. |
| [GetSortLeftToRight](./getsortlefttoright/) | True يعني أن اتجاه الفرز من اليسار إلى اليمين. False يعني أن اتجاه الفرز من الأعلى إلى الأسفل. القيمة الافتراضية هي false. |
| [SetSortLeftToRight](./setsortlefttoright/) | True يعني أن اتجاه الفرز من اليسار إلى اليمين. False يعني أن اتجاه الفرز من الأعلى إلى الأسفل. القيمة الافتراضية هي false. |
| [GetCaseSensitive](./getcasesensitive/) | يحصل ويضبط ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلسلة. |
| [SetCaseSensitive](./setcasesensitive/) | يحصل ويضبط ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلسلة. |
| [GetSortAsNumber](./getsortasnumber/) | يشير إلى ما إذا كان يتم فرز أي شيء يشبه الرقم. |
| [SetSortAsNumber](./setsortasnumber/) | يشير إلى ما إذا كان يتم فرز أي شيء يشبه الرقم. |
| [Sort_Cells_Int_Int_Int_Int](./sort_cells_int_int_int_int/) | يقوم بفرز بيانات المنطقة. |
| [Sort_Cells_CellArea](./sort_cells_cellarea/) | فرز بيانات المنطقة. |
| [Sort](./sort/) | فرز البيانات في النطاق. |
