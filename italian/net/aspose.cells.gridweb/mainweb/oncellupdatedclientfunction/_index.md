---
title: "MainWeb.OnCellUpdatedClientFunction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MainWeb. Ottiene o imposta il nome della funzione lato client da chiamare quando il valore di una cella viene aggiornato. La funzione client dovrebbe essere dichiarata così: function MyOnCellUpdatedcell  alertthis.getCellValueByCellcell Nota: è possibile utilizzare il puntatore this nella funzione client per fare riferimento al controllo griglia che genera l'evento"
type: docs
url: /it/net/aspose.cells.gridweb/mainweb/oncellupdatedclientfunction/
---
## MainWeb.OnCellUpdatedClientFunction property

Ottiene o imposta il nome della funzione lato client da chiamare quando il valore di una cella viene aggiornato. La funzione client deve essere dichiarata così: function MyOnCellUpdated(cell) { alert(this.getCellValueByCell(cell)); }Nota: è possibile utilizzare il puntatore \"this\" nella funzione client per fare riferimento al controllo della griglia che genera l'evento.

```csharp
public string OnCellUpdatedClientFunction { get; set; }
```

### Vedi anche

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


