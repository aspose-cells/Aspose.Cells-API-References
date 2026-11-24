---
title: "MainWeb.OnCellErrorClientFunction"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MainWeb Eigenschaft. Gibt den Namen der clientseitigen Funktion an, die aufgerufen wird, wenn die Validierung einer Zelle fehlschlägt. Die clientseitige Funktion sollte wie folgt deklariert werden: function MyOnCellErrorcell  alertthis.getCellValueByCellcell Hinweis: Sie können den this‑Zeiger in der clientseitigen Funktion verwenden, um das Rastersteuerelement zu referenzieren, das das Ereignis auslöst."
type: docs
url: /de/net/aspose.cells.gridweb/mainweb/oncellerrorclientfunction/
---
## MainWeb.OnCellErrorClientFunction property

Liest oder setzt den Namen der clientseitigen Funktion, die aufgerufen wird, wenn die Validierung einer Zelle fehlschlägt. Die Client‑Funktion sollte wie folgt deklariert werden: function MyOnCellError(cell) { alert(this.getCellValueByCell(cell)); } Hinweis: Sie können den \"this\"‑Zeiger in der Client‑Funktion verwenden, um auf das Grid‑Steuerelement zu verweisen, das das Ereignis auslöst.

```csharp
public string OnCellErrorClientFunction { get; set; }
```

### Siehe auch

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


