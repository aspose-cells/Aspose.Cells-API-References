---
title: "MainWeb.OnContextMenuShowClientFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MainWeb-Eigenschaft. Gibt die clientseitige Funktion an, die aufgerufen wird, wenn das Kontextmenü angezeigt wird, oder legt sie fest. Die clientseitige Funktion sollte wie folgt deklariert werden: function onContextMenuShow  var menu  event.srcElement menu.setItemVisibilityDelete block menu.setItemVisibilityUpdate none Hinweis: Sie können den this‑Pointer in der clientseitigen Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst."
type: docs
url: /de/net/aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/
---
## MainWeb.OnContextMenuShowClientFunction property

Legt die clientseitige Funktion fest, die aufgerufen wird, wenn das Kontextmenü angezeigt wird, oder ruft sie ab. Die Clientfunktion sollte wie folgt deklariert werden: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst.

```csharp
public string OnContextMenuShowClientFunction { get; set; }
```

### Siehe auch

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


