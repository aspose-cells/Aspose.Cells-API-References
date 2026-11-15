---
title: "فئة PivotCache"
linktitle: "PivotCache"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة PivotCache. تغلف الكائن الذي يمثل pivotcache في Go."
type: docs
weight: 200
url: /ar/go-cpp/pivotcache/
---

## PivotCache class

يمثل ذاكرة التخزين المؤقت لبعض تقارير PivotTable.

```go

type PivotCache struct  {
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
| [GetMissingItemsLimit](./getmissingitemslimit/) | يحصل ويضبط عدد العناصر غير المستخدمة المسموح بها قبل حذف العناصر غير المستخدمة. يجب أن تكون هذه القيمة أكبر من -2 وأقل من 1048577. PivotCacheMissingItemsLimitConst; |
| [SetMissingItemsLimit](./setmissingitemslimit/) | يحصل ويضبط عدد العناصر غير المستخدمة المسموح بها قبل حذف العناصر غير المستخدمة. يجب أن تكون هذه القيمة أكبر من -2 وأقل من 1048577. PivotCacheMissingItemsLimitConst; |
| [Refresh_PivotTableRefreshOption](./refresh_pivottablerefreshoption/) | يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات لعرض جميع جداول المحور التي يكون مصدر البيانات لها هذا PivotCache. |
| [Refresh](./refresh/) | يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات لعرض جميع جداول المحور التي يكون مصدر البيانات لها هذا PivotCache. |
| [GetPivotTables](./getpivottables/) | يحصل على جميع جداول المحور باستخدام هذا PivotCache. |
| [Dispose](./dispose/) | إطلاق جميع الموارد. |
| [GetSourceType](./getsourcetype/) | يحصل على PivotTableSourceType. |
