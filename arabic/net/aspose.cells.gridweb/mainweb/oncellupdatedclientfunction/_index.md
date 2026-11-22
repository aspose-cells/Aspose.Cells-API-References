---
title: "MainWeb.OnCellUpdatedClientFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MainWeb. تحصل أو تعيين اسم الدالة الجانبية التي تُستدعى عندما يتم تحديث قيمة خلية. يجب إعلان الدالة الجانبية هكذا function MyOnCellUpdatedcell  alertthis.getCellValueByCellcell ملاحظة يمكنك استخدام مؤشر this في الدالة الجانبية للإشارة إلى عنصر الشبكة الذي يطلق الحدث"
type: docs
url: /ar/net/aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/
---
## MainWeb.OnCellUpdatedClientFunction property

يحصل أو يعيّن اسم الدالة الجانبية للعميل التي يتم استدعاؤها عند تحديث قيمة الخلية. يجب إعلان دالة العميل هكذا: `function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); }` ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر الشبكة الذي يطلق الحدث.

```csharp
public string OnCellUpdatedClientFunction { get; set; }
```

### انظر أيضًا

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


