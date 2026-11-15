---
title: "فئة AutoFilter"
linktitle: "AutoFilter"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة AutoFilter. تغلف الكائن الذي يمثل الفلتر التلقائي في Go."
type: docs
weight: 200
url: /ar/go-cpp/autofilter/
---

## AutoFilter class

يمثل التصفية التلقائية للورقة المحددة.

```go

type AutoFilter struct  {
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
| [GetSorter](./getsorter/) | يحصل على مُرتّب البيانات. |
| [SetRange_Int_Int_Int](./setrange_int_int_int/) | يضبط النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [GetCellArea](./getcellarea/) | يحصل على CellArea الذي ينطبق عليه هذا AutoFilter. |
| [GetCellArea_Bool](./getcellarea_bool/) | يحصل على Aspose.Cells.CellArea حيث ينطبق AutoFilter المحدد. |
| [GetRange](./getrange/) | يمثل النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [SetRange_String](./setrange_string/) | يمثل النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [AddFilter](./addfilter/) | يضيف مرشحًا لعمود الفلترة. |
| [AddDateFilter](./adddatefilter/) | يضيف مرشح تاريخ. |
| [RemoveDateFilter](./removedatefilter/) | يزيل مرشح تاريخ. |
| [RemoveFilter_Int_String](./removefilter_int_string/) | يزيل مرشحًا لعمود الفلترة. |
| [Filter](./filter/) | يفلتر قائمة بالمعايير المحددة. |
| [FilterTop10](./filtertop10/) | فلتر أعلى 10 عناصر في القائمة |
| [Dynamic_Filter](./dynamic_filter/) | يضيف مرشحًا ديناميكيًا. |
| [AddFontColorFilter](./addfontcolorfilter/) | يضيف مرشح لون الخط. |
| [AddFillColorFilter](./addfillcolorfilter/) | يضيف مرشح لون التعبئة. |
| [AddIconFilter](./addiconfilter/) | يضيف مرشح أيقونة. |
| [MatchBlanks](./matchblanks/) | مطابقة جميع الخلايا الفارغة في القائمة. |
| [MatchNonBlanks](./matchnonblanks/) | مطابقة جميع الخلايا غير الفارغة في القائمة. |
| [Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | يفلتر قائمة بمعيار مخصص. |
| [Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | يفلتر قائمة بمعايير مخصصة. |
| [ShowAll](./showall/) | إظهار جميع الصفوف. |
| [RemoveFilter_Int](./removefilter_int/) | إزالة المرشح المحدد. |
| [Refresh](./refresh/) | تحديث الفلاتر التلقائية لإخفاء أو إظهار الصفوف. |
| [Refresh_Bool](./refresh_bool/) | يحصل على فهارس جميع الصفوف المخفية. |
| [GetShowFilterButton](./getshowfilterbutton/) | يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا. |
| [SetShowFilterButton](./setshowfilterbutton/) | يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا. |
| [GetFilterColumns](./getfiltercolumns/) | يحصل على مجموعة أعمدة الفلتر. |
