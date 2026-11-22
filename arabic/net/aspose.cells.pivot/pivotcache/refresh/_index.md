---
title: "PivotCache.Refresh"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotCache. تقوم بتحديث البيانات من مصدر البيانات وتحسب البيانات لعرض جميع جداول PivotTable التي مصدر بياناتها هو هذا PivotCache."
type: docs
url: /ar/net/aspose.cells.pivot/pivotcache/refresh/
---
## Refresh(PivotTableRefreshOption) {#refresh_1}

يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات لعرض جميع الجداول المحورية التي يكون مصدر بياناتها هذه الذاكرة المؤقتة.

```csharp
public PivotRefreshState Refresh(PivotTableRefreshOption option)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيار | PivotTableRefreshOption | الخيارات لتحديث مصدر بيانات جدول PivotTable. |

### ملاحظات

من الأفضل أن يمكنك ببساطة استدعاء [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) لتحديث جميع جداول PivotTable والرسوم البيانية في الملف.

### انظر أيضًا

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Refresh() {#refresh}

يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات لعرض جميع الجداول المحورية التي يكون مصدر بياناتها هذه الذاكرة المؤقتة.

```csharp
public PivotRefreshState Refresh()
```

### ملاحظات

إذا كان كل من table1 و table2 يستخدمان هذا التخزين المؤقت، سيتم حساب الجدولين. من الأفضل أن يمكنك ببساطة استدعاء [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) لتحديث جميع جداول PivotTable والرسوم البيانية في الملف.

### انظر أيضًا

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


