---
title: "CellErrorHandler"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la interfaz que pretende manejar eventos de error de celda."
type: docs
url: /es/java/com.aspose.gridweb/cellerrorhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellErrorHandler extends Serializable
```

Representa la interfaz que pretende manejar eventos de error de celda.
## Métodos

| Método | Descripción |
| --- | --- |
| [handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-) | manejar el evento de celda relacionado. |
### handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.GridCellException-com.aspose.gridweb.OnErrorActionQuery-}
```
public abstract void handleCellEvent(Object sender, GridCellException ex, OnErrorActionQuery query)
```


manejar el evento de celda relacionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | java.lang.Object | El origen del evento. |
| ex | [GridCellException](../../com.aspose.gridweb/gridcellexception) | El error de operación de la celda. |
| query | [OnErrorActionQuery](../../com.aspose.gridweb/onerroractionquery) | puede obtener información del tipo de acción onerror. |

