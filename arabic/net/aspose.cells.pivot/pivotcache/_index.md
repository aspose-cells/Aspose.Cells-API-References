---
title: "فئة PivotCache"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotCache. تمثل ذاكرة التخزين المؤقت للذاكرة لبعض تقارير PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivotcache/
---
## PivotCache class

يمثل ذاكرة التخزين المؤقت لبعض تقارير PivotTable.

```csharp
public abstract class PivotCache : IDisposable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [MissingItemsLimit](../../aspose.cells.pivot/pivotcache/missingitemslimit/) { get; set; } | يحصل على عدد العناصر غير المستخدمة المسموح بها قبل حذف العناصر غير المستخدمة ويضبطه. يجب أن تكون هذه القيمة أكبر من -2 وأقل من 1048577. [`PivotCacheMissingItemsLimitConst`](../pivotcachemissingitemslimitconst/); |
| abstract [SourceType](../../aspose.cells.pivot/pivotcache/sourcetype/) { get; } | يحصل على [`PivotTableSourceType`](../pivottablesourcetype/). |

## الطرق

| الاسم | الوصف |
| --- | --- |
| abstract [Dispose](../../aspose.cells.pivot/pivotcache/dispose/)() | تحرير جميع الموارد. |
| [GetPivotTables](../../aspose.cells.pivot/pivotcache/getpivottables/)() | يحصل على جميع الجداول المحورية باستخدام ذاكرة التخزين المؤقت هذه. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh)() | يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات لعرض جميع الجداول المحورية التي يكون مصدر بياناتها هذه الذاكرة المؤقتة. |
| [Refresh](../../aspose.cells.pivot/pivotcache/refresh/#refresh_1)(PivotTableRefreshOption) | يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات لعرض جميع الجداول المحورية التي يكون مصدر بياناتها هذه الذاكرة المؤقتة. |

### ملاحظات

سيتم جمع جميع البيانات في هذه الذاكرة المؤقتة، وستحصل الجداول المحورية على البيانات فقط من هذه الذاكرة ولا تصل مباشرة إلى مصدر البيانات. إذا كان مصدر بيانات بعض [`PivotTable`](../pivottable/)s هو نفسه، فستستخدم ذاكرة تخزين مؤقت محورية.

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


