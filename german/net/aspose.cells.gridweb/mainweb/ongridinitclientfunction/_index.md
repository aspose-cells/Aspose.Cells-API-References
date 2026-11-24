---
title: "MainWeb.OnGridInitClientFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MainWeb-Eigenschaft. Gibt den Namen der clientseitigen Funktion an, die aufgerufen wird, wenn das Raster initialisiert wird, oder legt ihn fest. Die clientseitige Funktion sollte wie folgt deklariert werden: function MyOnGridInitgrid  alert('Das Raster ist initialisiert')   grid.id Hinweis: Sie können den this‑Zeiger in der clientseitigen Funktion verwenden, um auf das Rastersteuerelement zu zeigen, das das Ereignis auslöst."
type: docs
url: /de/net/aspose.cells.gridweb/mainweb/ongridinitclientfunction/
---
## MainWeb.OnGridInitClientFunction property

Legt den Namen der clientseitigen Funktion fest, die aufgerufen wird, wenn das Grid initialisiert wird, oder ruft ihn ab. Die Clientfunktion sollte wie folgt deklariert werden: function MyOnGridInit(grid) { alert("The grid is initialized: " + grid.id); }Hinweis: Sie können den "this"-Zeiger in der Clientfunktion verwenden, um auf das Grid-Steuerelement zu verweisen, das das Ereignis auslöst.

```csharp
public string OnGridInitClientFunction { get; set; }
```

### Siehe auch

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


