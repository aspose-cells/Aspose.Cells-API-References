---
title: "WorkbookEventHandler"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'interfaccia che intende gestire gli eventi della cartella di lavoro."
type: docs
url: /it/java/com.aspose.gridweb/workbookeventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface WorkbookEventHandler extends Serializable
```

Rappresenta l'interfaccia che intende gestire gli eventi della cartella di lavoro.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | Gestisci l'evento Cell correlato. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract void handleCellEvent(Object sender, CellEventArgs e)
```


Gestisci l'evento Cell correlato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sender | java.lang.Object | La sorgente dell'evento. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | L'argomento dell'evento. |

