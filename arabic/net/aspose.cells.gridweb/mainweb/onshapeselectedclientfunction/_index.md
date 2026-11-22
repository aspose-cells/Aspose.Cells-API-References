---
title: "MainWeb.OnShapeSelectedClientFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "MainWeb الخاصية. يحصل أو يضبط الدالة الجانبية التي يتم استدعاؤها عند تحديد شكل. يجب إعلان الدالة الجانبية هكذا function MyOnSelectShapeshape  var nameshape.getAttributenamevalue var textshape.getAttributetextvalue var valueshape.getAttributecontrolvalue var typeshape.getAttributemsotype ملاحظة يمكنك استخدام مؤشر this في الدالة الجانبية للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث"
type: docs
url: /ar/net/aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/
---
## MainWeb.OnShapeSelectedClientFunction property

الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها عند تحديد شكل. يجب إعلان دالة العميل كما يلي: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

```csharp
public string OnShapeSelectedClientFunction { get; set; }
```

### انظر أيضًا

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


