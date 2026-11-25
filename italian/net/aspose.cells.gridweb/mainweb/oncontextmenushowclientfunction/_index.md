---
title: "MainWeb.OnContextMenuShowClientFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MainWeb property. Ottiene o imposta la funzione lato client da chiamare quando il menu contestuale viene mostrato. La funzione client dovrebbe essere dichiarata così function onContextMenuShow  var menu  event.srcElement menu.setItemVisibilityDelete block menu.setItemVisibilityUpdate none Nota È possibile utilizzare il puntatore this nella funzione client per fare riferimento al controllo grid che genera l'evento"
type: docs
url: /it/net/aspose.cells.gridweb/mainweb/oncontextmenushowclientfunction/
---
## MainWeb.OnContextMenuShowClientFunction property

Ottiene o imposta la funzione lato client da chiamare quando il menu contestuale verrà mostrato. La funzione client dovrebbe essere dichiarata così: function onContextMenuShow() { var menu = event.srcElement; menu.setItemVisibility("Delete", "block"); menu.setItemVisibility("Update", "none"); }Nota: è possibile utilizzare il puntatore "this" nella funzione client per puntare al controllo grid che genera l'evento.

```csharp
public string OnContextMenuShowClientFunction { get; set; }
```

### Vedi anche

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


