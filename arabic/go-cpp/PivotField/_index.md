---
title: "فئة PivotField"
linktitle: "PivotField"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PivotField. يضم الكائن الذي يمثل pivotfield في Go."
type: docs
weight: 200
url: /ar/go-cpp/pivotfield/
---

## PivotField class

يمثل حقلًا في تقرير PivotTable.

```go

type PivotField struct  {
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
| [GetPivotItems](./getpivotitems/) | يحصل على عناصر pivot للحقل المحوري. |
| [GetMaxValue](./getmaxvalue/) | يحصل على القيمة القصوى لهذا الحقل. |
| [GetMinValue](./getminvalue/) | يحصل على القيمة القصوى لهذا الحقل. |
| [GetGroupSettings](./getgroupsettings/) | يحصل على إعدادات المجموعة للحقل المحوري. |
| [InitPivotItems](./initpivotitems/) | تهيئة عناصر pivot للحقل المحوري. |
| [Group](./group/) | تجميع الحقل تلقائيًا. |
| [Group_PivotFieldGroupOptions](./group_pivotfieldgroupoptions/) | يقوم بتجميع الحقل المحوري مع الخيارات. |
| [GroupBy](./groupby/) | تجميع مخصص للحقل. |
| [Ungroup](./ungroup/) | إلغاء تجميع الحقل المحوري. |
| [GetPivotFilterByType](./getpivotfilterbytype/) | يحصل على مرشح المحور لحقل المحور حسب النوع |
| [GetFilters](./getfilters/) | يسترجع جميع مرشحات المحور المطبقة لهذا الحقل المحوري. |
| [ClearFilter](./clearfilter/) | يمسح إعدادات المرشح لهذا الحقل المحوري. |
| [FilterTop10](./filtertop10/) | يفلتر حسب قيم حقل pivot field للبيانات. |
| [FilterByValue](./filterbyvalue/) | يفلتر حسب قيم حقل pivot field للبيانات. |
| [FilterByLabel](./filterbylabel/) | يفلتر حسب عناوين صف أو عمود حقل pivot field. |
| [FilterByDate](./filterbydate/) | يفلتر حسب قيم التاريخ لحقل المحور الصف أو العمود. |
| [IsCalculatedField](./iscalculatedfield/) | يحدد ما إذا كان هذا الحقل المحوري حقلًا محسوبًا. |
| [GetFormula](./getformula/) | يسترجع صيغة الحقل المحسوب. يعمل فقط مع الحقول المحسوبة. |
| [IsValuesField](./isvaluesfield/) | يحدد ما إذا كان هذا الحقل يمثل حقل القيم. |
| [GetBaseIndex](./getbaseindex/) | يمثل الفهرس في حقول المحور المصدر. |
| [SetBaseIndex](./setbaseindex/) | يمثل الفهرس في حقول المحور المصدر. |
| [GetPosition](./getposition/) | يمثل فهرس حقل المحور في المنطقة. |
| [GetRegionType](./getregiontype/) | يحدد منطقة جدول المحور التي يُعرض فيها هذا الحقل. |
| [GetName](./getname/) | يمثل اسم حقل المحور. |
| [SetName](./setname/) | يمثل اسم حقل المحور. |
| [GetDisplayName](./getdisplayname/) | يمثل الاسم المعروض لحقل المحور في عرض جدول المحور. |
| [SetDisplayName](./setdisplayname/) | يمثل الاسم المعروض لحقل المحور في عرض جدول المحور. |
| [SetSubtotals_PivotFieldSubtotalType_Bool](./setsubtotals_pivotfieldsubtotaltype_bool/) | يحدد كيفية تجميع الحقل المحدد. |
| [GetSubtotals_PivotFieldSubtotalType](./getsubtotals_pivotfieldsubtotaltype/) | يحدد ما إذا كان سيتم إظهار التجميع الفرعي المحدد لهذا الحقل المحوري. |
| [GetSubtotals](./getsubtotals/) | يسترجع أو يضبط التجميعات الفرعية للحقل. يخص فقط حقول المحور الصفية أو العمودية. |
| [SetSubtotals_PivotFieldSubtotalType](./setsubtotals_pivotfieldsubtotaltype/) | يسترجع أو يضبط التجميعات الفرعية للحقل. يخص فقط حقول المحور الصفية أو العمودية. |
| [IsAutoSubtotals](./isautosubtotals/) | يحدد ما إذا كان الحقل المحدد يظهر تجميعات فرعية تلقائية. القيمة الافتراضية هي true. |
| [SetIsAutoSubtotals](./setisautosubtotals/) | يحدد ما إذا كان الحقل المحدد يظهر تجميعات فرعية تلقائية. القيمة الافتراضية هي true. |
| [GetAllowDraggingToRow](./getallowdraggingtorow/) | يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. القيمة الافتراضية هي true. |
| [SetAllowDraggingToRow](./setallowdraggingtorow/) | يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصف. القيمة الافتراضية هي true. |
| [GetAllowDraggingToColumn](./getallowdraggingtocolumn/) | يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. القيمة الافتراضية هي true. |
| [SetAllowDraggingToColumn](./setallowdraggingtocolumn/) | يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة العمود. القيمة الافتراضية هي true. |
| [GetAllowDraggingToPage](./getallowdraggingtopage/) | يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. القيمة الافتراضية هي true. |
| [SetAllowDraggingToPage](./setallowdraggingtopage/) | يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة الصفحة. القيمة الافتراضية هي true. |
| [GetAllowRemovingFromView](./getallowremovingfromview/) | يحدد ما إذا كان يمكن إزالة هذا الحقل المحوري من عرض جدول المحور. القيمة الافتراضية هي true. |
| [SetAllowRemovingFromView](./setallowremovingfromview/) | يحدد ما إذا كان يمكن إزالة هذا الحقل المحوري من عرض جدول المحور. القيمة الافتراضية هي true. |
| [GetAllowDraggingToData](./getallowdraggingtodata/) | يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. القيمة الافتراضية هي true. |
| [SetAllowDraggingToData](./setallowdraggingtodata/) | يحدد ما إذا كان يمكن سحب الحقل المحدد إلى منطقة القيم. القيمة الافتراضية هي true. |
| [IsMultipleItemSelectionAllowed](./ismultipleitemselectionallowed/) | يحدد ما إذا كان يمكن اختيار عناصر متعددة في حقل الصفحة. القيمة الافتراضية هي false. |
| [SetIsMultipleItemSelectionAllowed](./setismultipleitemselectionallowed/) | يحدد ما إذا كان يمكن اختيار عناصر متعددة في حقل الصفحة. القيمة الافتراضية هي false. |
| [IsRepeatItemLabels](./isrepeatitemlabels/) | يحدد ما إذا كان يجب تكرار تسميات الحقل في المنطقة. القيمة الافتراضية هي false. |
| [SetIsRepeatItemLabels](./setisrepeatitemlabels/) | يحدد ما إذا كان يجب تكرار تسميات الحقل في المنطقة. القيمة الافتراضية هي false. |
| [IsIncludeNewItemsInFilter](./isincludenewitemsinfilter/) | يحدد ما إذا كان يجب تضمين عناصر جديدة إلى الحقل في الفلتر اليدوي. القيمة الافتراضية هي false. |
| [SetIsIncludeNewItemsInFilter](./setisincludenewitemsinfilter/) | يحدد ما إذا كان يجب تضمين عناصر جديدة إلى الحقل في الفلتر اليدوي. القيمة الافتراضية هي false. |
| [IsInsertPageBreaksBetweenItems](./isinsertpagebreaksbetweenitems/) | يحدد ما إذا كان يجب إدراج فواصل صفحات بعد كل عنصر. القيمة الافتراضية هي false. |
| [SetIsInsertPageBreaksBetweenItems](./setisinsertpagebreaksbetweenitems/) | يحدد ما إذا كان يجب إدراج فواصل صفحات بعد كل عنصر. القيمة الافتراضية هي false. |
| [GetShowAllItems](./getshowallitems/) | يشير إلى ما إذا كان يجب عرض جميع العناصر في عرض PivotTable، حتى إذا لم تحتوي على بيانات ملخص. القيمة الافتراضية هي false. |
| [SetShowAllItems](./setshowallitems/) | يشير إلى ما إذا كان يجب عرض جميع العناصر في عرض PivotTable، حتى إذا لم تحتوي على بيانات ملخص. القيمة الافتراضية هي false. |
| [SortBy_SortOrder](./sortby_sortorder/) | يقوم بفرز هذا الحقل المحوري. |
| [SortBy_SortOrder_Int_String](./sortby_sortorder_int_string/) | يقوم بفرز هذا الحقل المحوري. |
| [GetSortSetting](./getsortsetting/) | يحصل على جميع إعدادات الفرز التلقائي |
| [GetTop10AutoShowSettings](./gettop10autoshowsettings/) | يحصل على إعدادات Top 10 AutoShow لحقل محوري. |
| [Top10AutoShow](./top10autoshow/) | يضبط إعدادات Top10 AutoShow لهذا الحقل المحوري. |
| [GetFunction](./getfunction/) | يمثل الدالة المستخدمة لتلخيص حقل بيانات هذا PivotTable. |
| [SetFunction](./setfunction/) | يمثل الدالة المستخدمة لتلخيص حقل بيانات هذا PivotTable. |
| [ShowValuesAs](./showvaluesas/) | يعرض قيم حقل البيانات بصيغة عرض مختلفة عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [GetShowValuesSetting](./getshowvaluessetting/) | يحصل على إعدادات عرض القيم عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [GetCurrentPageItem](./getcurrentpageitem/) | يمثل عنصر الصفحة المحدد حاليًا لحقل الصفحة لتصفية البيانات. صالح فقط لحقول الصفحة. |
| [SetCurrentPageItem](./setcurrentpageitem/) | يمثل عنصر الصفحة المحدد حاليًا لحقل الصفحة لتصفية البيانات. صالح فقط لحقول الصفحة. |
| [GetInsertBlankRow](./getinsertblankrow/) | يشير إلى ما إذا كان يجب إدراج سطر فارغ بعد كل عنصر. فقط لحقول الصف. |
| [SetInsertBlankRow](./setinsertblankrow/) | يشير إلى ما إذا كان يجب إدراج سطر فارغ بعد كل عنصر. فقط لحقول الصف. |
| [GetShowSubtotalAtTop](./getshowsubtotalattop/) | يشير إلى ما إذا كان يجب عرض المجاميع الفرعية في أعلى أو أسفل العناصر عندما يكون ShowInOutlineForm صحيحًا، ثم |
| [SetShowSubtotalAtTop](./setshowsubtotalattop/) | يشير إلى ما إذا كان يجب عرض المجاميع الفرعية في أعلى أو أسفل العناصر عندما يكون ShowInOutlineForm صحيحًا، ثم |
| [GetShowInOutlineForm](./getshowinoutlineform/) | يشير إلى ما إذا كان يجب تنظيم هذا الحقل في شكل مخطط على عرض Pivot Table. |
| [SetShowInOutlineForm](./setshowinoutlineform/) | يشير إلى ما إذا كان يجب تنظيم هذا الحقل في شكل مخطط على عرض Pivot Table. |
| [GetNumber](./getnumber/) | يمثل تنسيق العرض المدمج للأرقام والتواريخ. |
| [SetNumber](./setnumber/) | يمثل تنسيق العرض المدمج للأرقام والتواريخ. |
| [Get_NumberFormat](./get_numberformat/) | يمثل تنسيق العرض المخصص للأرقام والتواريخ. |
| [SetNumberFormat](./setnumberformat/) | يمثل تنسيق العرض المخصص للأرقام والتواريخ. |
| [HideAllDetails](./hidealldetails/) | يخفي جميع التفاصيل |
| [ShowAllDetails](./showalldetails/) | إظهار جميع التفاصيل |
| [GetItems](./getitems/) | احصل على جميع تسميات عناصر المحور في هذا الحقل. |
| [GetOriginalItems](./getoriginalitems/) | احصل على العناصر الأساسية الأصلية؛ |
| [AddCalculatedItem](./addcalculateditem/) | أضف عنصر صيغة محسوبة إلى الحقل المحوري. |
| [GetShowCompact](./getshowcompact/) | يشير إلى ما إذا كان يجب عرض تسميات الحقل التالي في نفس العمود على عرض Pivot Table |
| [SetShowCompact](./setshowcompact/) | يشير إلى ما إذا كان يجب عرض تسميات الحقل التالي في نفس العمود على عرض Pivot Table |
