---
title: "RowColumnEventHandler"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'interfaccia che intende gestire gli eventi di righe/colonne."
type: docs
url: /it/java/com.aspose.gridweb/rowcolumneventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```

Rappresenta l'interfaccia che intende gestire gli eventi di righe/colonne.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | Gestisci l'evento Cell correlato. |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```


Gestisci l'evento Cell correlato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sender | java.lang.Object | La sorgente dell'evento. |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | L'argomento dell'evento. Chiama e.RejectOperation() se desideri annullare l'operazione di eliminazione nei gestori di eventi RowDeleting o ColumnDeleting. |

