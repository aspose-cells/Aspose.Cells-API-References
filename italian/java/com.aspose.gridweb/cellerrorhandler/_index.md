---
title: "CellErrorHandler"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'interfaccia che intende gestire gli eventi di errore delle celle."
type: docs
url: /it/java/com.aspose.gridweb/cellerrorhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```

Rappresenta l'interfaccia che intende gestire gli eventi di errore delle celle.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | Gestisci l'evento Cell correlato. |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```


Gestisci l'evento Cell correlato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sender | java.lang.Object | La sorgente dell'evento. |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | L'errore di operazione della cella. |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | può ottenere informazioni sul tipo di azione onerror. |

