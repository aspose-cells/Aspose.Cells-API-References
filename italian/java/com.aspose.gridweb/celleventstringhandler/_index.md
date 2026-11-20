---
title: "CellEventStringHandler"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'interfaccia che intende gestire gli eventi delle celle."
type: docs
url: /it/java/com.aspose.gridweb/celleventstringhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```

Rappresenta l'interfaccia che intende gestire gli eventi delle celle.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | Gestisci l'evento Cell correlato. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```


Gestisci l'evento Cell correlato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sender | java.lang.Object | La griglia di origine dell'evento. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | L'argomento dell'evento. e.Cell è la cella che genera l'evento. e.Argument contiene l'argomento dell'evento. |

**Returns:**
java.lang.String - valore stringa
