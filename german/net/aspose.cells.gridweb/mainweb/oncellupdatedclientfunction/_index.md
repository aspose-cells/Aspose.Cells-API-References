---
title: "MainWeb.OnCellUpdatedClientFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MainWeb-Eigenschaft. Gibt den Namen der clientseitigen Funktion an, die aufgerufen wird, wenn der Wert einer Zelle aktualisiert wird, oder legt ihn fest. Die clientseitige Funktion sollte wie folgt deklariert werden: function MyOnCellUpdatedcell  alert(this.getCellValueByCellcell) Hinweis: Sie können den this‑Zeiger in der clientseitigen Funktion verwenden, um auf das Rastersteuerelement zu zeigen, das das Ereignis auslöst."
type: docs
url: /de/net/aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/
---
## MainWeb.OnCellUpdatedClientFunction property

Liest oder setzt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn der Wert einer Zelle aktualisiert wird. Die Client‑Funktion sollte wie folgt deklariert werden: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); } Hinweis: Sie können den \"this\"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

```csharp
public string OnCellUpdatedClientFunction { get; set; }
```

### Siehe auch

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


