---
title: "MainWeb.OnContextMenuShowClientFunction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MainWeb propiedad. Obtiene o establece la función del lado del cliente que se llamará cuando se muestre el menú contextual. La función del cliente debe declararse así: function onContextMenuShow  var menu  event.srcElement menu.setItemVisibilityDelete block menu.setItemVisibilityUpdate none Nota: Puede usar el puntero this en la función del cliente para referirse al control de cuadrícula que dispara el evento"
type: docs
url: /es/net/aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/
---
## MainWeb.OnContextMenuShowClientFunction property

Obtiene o establece la función del lado del cliente que se llamará cuando se muestre el menú contextual. La función del cliente debe declararse así: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Nota: Puede usar el puntero "this" en la función del cliente para referirse al control de cuadrícula que dispara el evento.

```csharp
public string OnContextMenuShowClientFunction { get; set; }
```

### Ver también

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


