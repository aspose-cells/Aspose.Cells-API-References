---
title: MainWeb.OnContextMenuShowClientFunction
second_title: Aspose.Cells for .NET API Reference
description: MainWeb property. Gets or sets the client side function to be called when the context menu will be shown. The client function should be declared like this function onContextMenuShow  var menu  event.srcElement menu.setItemVisibilityDelete block menu.setItemVisibilityUpdate none Note You may use the this pointer in the client function to point the grid control which fires the event
type: docs
url: /net/aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/
---
## MainWeb.OnContextMenuShowClientFunction property

Gets or sets the client side function to be called when the context menu will be shown. The client function should be declared like this: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Note: You may use the "this" pointer in the client function to point the grid control which fires the event.

```csharp
public string OnContextMenuShowClientFunction { get; set; }
```

### See Also

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


