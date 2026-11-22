---
title: "MainWeb.OnCellErrorClientFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MainWeb. تحصل أو تعيين اسم الدالة من جانب العميل التي تُستدعى عندما يفشل التحقق من صحة خلية. يجب إعلان الدالة العميلة هكذا: function MyOnCellErrorcell  alertthis.getCellValueByCellcell ملاحظة: يمكنك استخدام مؤشر this في الدالة العميلة للإشارة إلى عنصر التحكم Grid الذي يطلق الحدث."
type: docs
url: /ar/net/aspose.cells.gridweb/mainweb/oncellerrorclientfunction/
---
## MainWeb.OnCellErrorClientFunction property

يحصل أو يعيّن اسم الدالة الجانبية للعميل التي يتم استدعاؤها عندما تفشل عملية التحقق من صحة الخلية. يجب إعلان دالة العميل هكذا: `function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); }` ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر الشبكة الذي يطلق الحدث.

```csharp
public string OnCellErrorClientFunction { get; set; }
```

### انظر أيضًا

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


