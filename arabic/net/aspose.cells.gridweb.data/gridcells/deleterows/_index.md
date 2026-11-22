---
title: "GridCells.DeleteRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridCells. تحذف عدة صفوف"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridcells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

يحذف عدة صفوف.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف الأول الذي سيُحذف. |
| totalRows | Int32 | عدد الصفوف التي سيتم حذفها. |

### ملاحظات

إذا كان النطاق المحذوف يحتوي على الجزء العلوي (ليس كاملًا) من الجدول (ListObject)، لا يمكن حذف النطاق ولن يتم أي شيء. يعمل كما في MS Excel.

### انظر أيضًا

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_1}

يحذف عدة صفوف في ورقة العمل.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف. |
| totalRows | Int32 | عدد الصفوف التي سيتم حذفها. |
| updateReference | منطقي | يشير إلى ما إذا كان يتم تحديث المراجع في أوراق العمل الأخرى. |

### انظر أيضًا

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


