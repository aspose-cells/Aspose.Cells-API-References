---
title: "PivotCache.CreatePivotTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotCache. تُنشئ تقرير PivotTable إلى ورقة جديدة"
type: docs
url: /ar/net/aspose.cells.gridweb.data/pivotcache/createpivottable/
---
## CreatePivotTable() {#createpivottable}

ينشئ تقرير PivotTable إلى ورقة جديدة.

```csharp
public PivotTable CreatePivotTable()
```

### قيمة الإرجاع

كائن PivotTable

### ملاحظات

ستؤدي استدعاء هذه الطريقة إلى إنشاء كائن PivotTable وورقة عمل جديدة. ثم تُضيف كائن PivotTable إلى الموقع الأخير في GridWeb.Worksheets.PivotTables. إذا قمت باستدعاء طريقة PivotTable.DataBind()، سيتم رسم تقرير PivotTable على ورقة العمل التي تم إنشاؤها.

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(string) {#createpivottable_3}

ينشئ تقرير PivotTable إلى ورقة جديدة. اسم كائن pivotTable

```csharp
public PivotTable CreatePivotTable(string tableName)
```

### قيمة الإرجاع

كائن PivotTable

### ملاحظات

ستؤدي استدعاء هذه الطريقة إلى إنشاء كائن PivotTable وورقة عمل جديدة. ثم تُضيف كائن PivotTable إلى الموقع الأخير في GridWeb.Worksheets.PivotTables. إذا قمت باستدعاء طريقة PivotTable.DataBind()، سيتم رسم تقرير PivotTable على ورقة العمل التي تم إنشاؤها.

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell) {#createpivottable_1}

ينشئ تقرير PivotTable إلى targetSheet.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| targetSheet | WebWorksheet | الورقة التي سيُرسم عليها تقرير pivotTable |
| targetCell | WebCell | خلية البداية التي سيُرسم عليها تقرير pivotTable |

### قيمة الإرجاع

كائن PivotTable

### ملاحظات

ستؤدي استدعاء هذه الطريقة إلى إنشاء كائن PivotTable ثم تُضيف كائن PivotTable إلى الموقع الأخير في GridWeb.Worksheets.PivotTables. إذا قمت باستدعاء طريقة PivotTable.DataBind()، سيتم رسم تقرير PivotTable على targetSheet بدءًا من targetCell.

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## CreatePivotTable(WebWorksheet, WebCell, string) {#createpivottable_2}

ينشئ تقرير PivotTable إلى targetSheet.

```csharp
public PivotTable CreatePivotTable(WebWorksheet targetSheet, WebCell targetCell, string tableName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| targetSheet | WebWorksheet | الورقة التي سيُرسم عليها تقرير pivotTable |
| targetCell | WebCell | خلية البداية التي سيُرسم عليها تقرير pivotTable |
| tableName | String | اسم كائن pivotTable |

### قيمة الإرجاع

كائن PivotTable

### ملاحظات

ستؤدي استدعاء هذه الطريقة إلى إنشاء كائن PivotTable باسم tableName ثم تُضيف كائن PivotTable إلى الموقع الأخير في GridWeb.Worksheets.PivotTables. إذا قمت باستدعاء طريقة PivotTable.DataBind()، سيتم رسم تقرير PivotTable على targetSheet بدءًا من targetCell.

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [WebWorksheet](../../webworksheet/)
* class [WebCell](../../webcell/)
* class [PivotCache](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


