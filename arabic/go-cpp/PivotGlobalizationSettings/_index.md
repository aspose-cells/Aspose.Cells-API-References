---
title: "فئة PivotGlobalizationSettings"
linktitle: "PivotGlobalizationSettings"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PivotGlobalizationSettings. تغلف الكائن الذي يمثل pivotglobalizationsettings في Go."
type: docs
weight: 200
url: /ar/go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

يمثل إعدادات العولمة لجداول المحور.

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | البناء الافتراضي. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetTextOfTotal](./gettextoftotal/) | يحصل على نص تسمية "Total" في PivotTable. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي PivotTable على حقلين PivotFields أو أكثر في منطقة البيانات. |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | يحصل على نص تسمية "Grand Total" في PivotTable. |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | يحصل على نص تسمية "(Multiple Items)" في PivotTable. |
| [GetTextOfAll](./gettextofall/) | يحصل على نص تسمية "(All)" في PivotTable. |
| [GetTextOfProtectedName](./gettextofprotectedname/) | يحصل على النص للاسم المحمي المحدد. |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | يحصل على نص تسمية "Column Labels" في PivotTable. |
| [GetTextOfRowLabels](./gettextofrowlabels/) | يحصل على نص تسمية "Row Labels" في PivotTable. |
| [GetTextOfEmptyData](./gettextofemptydata/) | يحصل على نص تسمية "(blank)" في PivotTable. |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | يحصل على نص رأس حقل منطقة القيمة في PivotTable. |
| [GetShortTextOf12Months](./getshorttextof12months/) | يحصل على جميع السلاسل ذات التنسيق القصير لـ 12 شهرًا. |
| [GetTextOf24Hours](./gettextof24hours/) | يحصل على جميع السلاسل ذات التنسيق المحلي لـ 24 ساعة. القيمة الافتراضية هي 12 ص، 1 ص، 2 ص، 3 ص، 4 ص، 5 ص، 6 ص، 7 ص، 8 ص، 9 ص، 10 ص، 11 ص، 12 م، 1 م، 2 م، 3 م، 4 م، 5 م، 6 م، 7 م، 8 م، 9 م، 10 م، 11 م. |
| [GetTextOfOr](./gettextofor/) | يحصل على جميع السلاسل ذات التنسيق المحلي لكلمة "or". |
| [GetFormatOfDayGroup](./getformatofdaygroup/) | يحصل على تنسيق الرقم لمجموعة أيام المحور. يستخدم فقط عند تجميع حقل المحور حسب الأيام. القيمة الافتراضية هي "d-MMM"; |
| [GetTextOf4Quaters](./gettextof4quaters/) | يحصل على النص المحلي لـ 4 أرباع. |
| [GetTextOf4Quarters](./gettextof4quarters/) | يحصل على النص المحلي لـ 4 أرباع. |
| [GetTextOfYears](./gettextofyears/) | يحصل على النص المحلي لكلمة "Years". |
| [GetTextOfQuarters](./gettextofquarters/) | احصل على النص المحلي لـ "Quarters". |
| [GetTextOfMonths](./gettextofmonths/) | يحصل على النص المحلي لـ "Months". |
| [GetTextOfDays](./gettextofdays/) | يحصل على النص المحلي لـ "Days". |
| [GetTextOfHours](./gettextofhours/) | يحصل على النص المحلي لـ "Hours". |
| [GetTextOfMinutes](./gettextofminutes/) | يحصل على النص المحلي لـ "Minutes". |
| [GetTextOfSeconds](./gettextofseconds/) | يحصل على النص المحلي لـ "Seconds" |
| [GetTextOfRange](./gettextofrange/) | يحصل على النص المحلي لـ "Range" |
| [GetTextOfAllPeriods](./gettextofallperiods/) | يحصل على النص المحلي لـ "All Periods" |
| [GetTextOfSubTotal](./gettextofsubtotal/) | يحصل على نص النوع PivotFieldSubtotalType في PivotTable. |
| [GetNameOfDataField](./getnameofdatafield/) | يحصل على اسم العرض لحقل محور البيانات.التنسيق الافتراضي هو "Sum Of Field". |
