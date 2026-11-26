---
title: "MainWeb.OnShapeSelectedClientFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MainWeb. Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una forma. La función del cliente debe declararse así: function MyOnSelectShapeshape  var nameshape.getAttributenamevalue var textshape.getAttributetextvalue var valueshape.getAttributecontrolvalue var typeshape.getAttributemsotype Nota: Puede usar el puntero this en la función del cliente para referirse al control de cuadrícula que dispara el evento."
type: docs
url: /es/net/aspose.cells.gridweb/mainweb/onshapeselectedclientfunction/
---
## MainWeb.OnShapeSelectedClientFunction property

Obtiene o establece la función del lado del cliente que se llamará cuando se seleccione una forma. La función del cliente debe declararse así: function MyOnSelectShape(shape) { var name=shape.getAttribute("namevalue") var text=shape.getAttribute("textvalue") var value=shape.getAttribute("controlvalue") var type=shape.getAttribute("msotype") }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

```csharp
public string OnShapeSelectedClientFunction { get; set; }
```

### Ver también

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


