---
title: "RowColumnEventHandler"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la interfaz que pretende manejar eventos de fila/columna."
type: docs
url: /es/java/com.aspose.gridweb/rowcolumneventhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface RowColumnEventHandler extends Serializable
```

Representa la interfaz que pretende manejar eventos de fila/columna.
## Métodos

| Método | Descripción |
| --- | --- |
| [handleCellEvent(Object sender, RowColumnEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-) | manejar el evento de celda relacionado. |
### handleCellEvent(Object sender, RowColumnEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.RowColumnEventArgs-}
```
public abstract void handleCellEvent(Object sender, RowColumnEventArgs e)
```


manejar el evento de celda relacionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | java.lang.Object | El origen del evento. |
| e | [RowColumnEventArgs](../../com.aspose.gridweb/rowcolumneventargs) | El argumento del evento. Llame a e.RejectOperation() si desea cancelar la operación de eliminación en los controladores de eventos RowDeleting o ColumnDeleting. |

