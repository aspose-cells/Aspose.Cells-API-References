---
title: "MainWeb.OnContextMenuShowClientFunction"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MainWeb property. Hämtar eller anger den klientsidiga funktionen som ska anropas när snabbmenyn visas. Klientfunktionen bör deklareras så här function onContextMenuShow  var menu  event.srcElement menu.setItemVisibilityDelete block menu.setItemVisibilityUpdate none Notera att du kan använda this‑pekaren i klientfunktionen för att referera till rutnätkontrollen som utlöser händelsen"
type: docs
url: /sv/net/aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/
---
## MainWeb.OnContextMenuShowClientFunction property

Hämtar eller anger den klientsidiga funktionen som ska anropas när snabbmenyn ska visas. Klientfunktionen bör deklareras så här: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Obs: Du kan använda "this"-pekaren i klientfunktionen för att peka på gridkontrollen som utlöser händelsen.

```csharp
public string OnContextMenuShowClientFunction { get; set; }
```

### Se även

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


