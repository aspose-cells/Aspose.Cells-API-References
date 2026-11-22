---
title: "MainWeb.OnContextMenuShowClientFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MainWeb. تحصل أو تعيين الدالة الجانبية التي تُستدعى عند إظهار قائمة السياق. يجب إعلان الدالة العميلة هكذا function onContextMenuShow  var menu  event.srcElement menu.setItemVisibilityDelete block menu.setItemVisibilityUpdate none ملاحظة يمكنك استخدام المؤشر this في الدالة العميلة للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث"
type: docs
url: /ar/net/aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/
---
## MainWeb.OnContextMenuShowClientFunction property

الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها عندما يتم عرض قائمة السياق. يجب إعلان دالة العميل كما يلي: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

```csharp
public string OnContextMenuShowClientFunction { get; set; }
```

### انظر أيضًا

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


