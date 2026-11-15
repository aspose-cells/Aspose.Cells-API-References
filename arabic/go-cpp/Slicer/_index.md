---
title: "فئة المقطّع"
linktitle: "المقطّع"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة المقطّع. تغلف الكائن الذي يمثل المقطّع في Go."
type: docs
weight: 200
url: /ar/go-cpp/slicer/
---

## Slicer class

وصف موجز لـ Slicer View

```go

type Slicer struct  {
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
| [GetSortOrderType](./getsortordertype/) | يحدد نوع فرز العناصر. |
| [SetSortOrderType](./setsortordertype/) | يحدد نوع فرز العناصر. |
| [GetShowMissing](./getshowmissing/) | يحدد ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات. |
| [SetShowMissing](./setshowmissing/) | يحدد ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات. |
| [GetShowTypeOfItemsWithNoData](./getshowtypeofitemswithnodata/) | يحدد ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات. |
| [SetShowTypeOfItemsWithNoData](./setshowtypeofitemswithnodata/) | يحدد ما إذا كان يجب عرض العناصر المحذوفة من مصدر البيانات. |
| [GetShowAllItems](./getshowallitems/) | يحدد ما إذا كان يجب عرض جميع العناصر حتى إذا لم تكن هناك بيانات أو تم حذفها. القيمة الافتراضية هي true؛ |
| [SetShowAllItems](./setshowallitems/) | يحدد ما إذا كان يجب عرض جميع العناصر حتى إذا لم تكن هناك بيانات أو تم حذفها. القيمة الافتراضية هي true؛ |
| [AddPivotConnection](./addpivotconnection/) | يضيف اتصال PivotTable. |
| [RemovePivotConnection](./removepivotconnection/) | يزيل اتصال PivotTable. |
| [GetLockedPosition](./getlockedposition/) | يحدد ما إذا كان يمكن نقل المقطّع المحدد أو تغيير حجمه باستخدام واجهة المستخدم. |
| [SetLockedPosition](./setlockedposition/) | يحدد ما إذا كان يمكن نقل المقطّع المحدد أو تغيير حجمه باستخدام واجهة المستخدم. |
| [Refresh](./refresh/) | تحديث عناصر المقطّع من جداول Pivot المرتبطة. |
| [GetShape](./getshape/) | يعيد كائن Shape المرتبط بالمقطّع المحدد. قراءة فقط. |
| [GetSlicerCache](./getslicercache/) | يعيد كائن SlicerCache المرتبط بالمقطّع. قراءة فقط. |
| [GetWorksheet](./getworksheet/) | يعيد كائن Worksheet الذي يحتوي على هذا المقطّع. قراءة فقط. |
| [GetStyleType](./getstyletype/) | حدد نوع نمط المقطّع المدمج. النوع الافتراضي هو SlicerStyleLight1. |
| [SetStyleType](./setstyletype/) | حدد نوع نمط المقطّع المدمج. النوع الافتراضي هو SlicerStyleLight1. |
| [GetName](./getname/) | يعيد أو يضبط اسم المقطّع المحدد |
| [SetName](./setname/) | يعيد أو يضبط اسم المقطّع المحدد |
| [GetCaption](./getcaption/) | يعيد أو يضبط تسمية المقطّع المحدد. |
| [SetCaption](./setcaption/) | يعيد أو يضبط تسمية المقطّع المحدد. |
| [GetFirstItemIndex](./getfirstitemindex/) | يحدد الفهرس الصفري للعنصر الأول في المقطّع. |
| [SetFirstItemIndex](./setfirstitemindex/) | يحدد الفهرس الصفري للعنصر الأول في المقطّع. |
|[SelectItems](./selectitems/) |  | 
| [UnselectItems](./unselectitems/) | إزالة تسميات الفلاتر المحددة. |
| [ClearFilter](./clearfilter/) | إزالة الفلاتر |
| [GetShowCaption](./getshowcaption/) | يحدد ما إذا كان رأس المقطّع مرئيًا. القيمة الافتراضية هي true |
| [SetShowCaption](./setshowcaption/) | يحدد ما إذا كان رأس المقطّع مرئيًا. القيمة الافتراضية هي true |
| [GetNumberOfColumns](./getnumberofcolumns/) | يعيد أو يضبط عدد الأعمدة في المقطّع. القيمة الافتراضية هي 1. |
| [SetNumberOfColumns](./setnumberofcolumns/) | يعيد أو يضبط عدد الأعمدة في المقطّع. القيمة الافتراضية هي 1. |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | يحصل أو يضبط عرض كل عمود في المقطّع، بوحدة البكسل. |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | يحصل أو يضبط عرض كل عمود في المقطّع، بوحدة البكسل. |
| [GetColumnWidth](./getcolumnwidth/) | يعيد أو يضبط عرض كل عمود في المقطّع بوحدة النقاط. |
| [SetColumnWidth](./setcolumnwidth/) | يعيد أو يضبط عرض كل عمود في المقطّع بوحدة النقاط. |
| [GetRowHeightPixel](./getrowheightpixel/) | يعيد أو يضبط ارتفاع كل صف في المقطّع المحدد، بوحدة البكسل. |
| [SetRowHeightPixel](./setrowheightpixel/) | يعيد أو يضبط ارتفاع كل صف في المقطّع المحدد، بوحدة البكسل. |
| [GetRowHeight](./getrowheight/) | يعيد أو يضبط ارتفاع كل صف في المقطّع المحدد بوحدة النقاط. |
| [SetRowHeight](./setrowheight/) | يعيد أو يضبط ارتفاع كل صف في المقطّع المحدد بوحدة النقاط. |
