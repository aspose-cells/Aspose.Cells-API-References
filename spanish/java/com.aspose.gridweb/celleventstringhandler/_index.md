---
title: "CellEventStringHandler"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la interfaz que pretende manejar eventos de celda."
type: docs
url: /es/java/com.aspose.gridweb/celleventstringhandler/
---

**All Implemented Interfaces:**
java.io.Serializable
```
public interface CellEventStringHandler extends Serializable
```

Representa la interfaz que pretende manejar eventos de celda.
## Métodos

| Método | Descripción |
| --- | --- |
| [handleCellEvent(Object sender, CellEventArgs e)](#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-) | manejar el evento de celda relacionado. |
### handleCellEvent(Object sender, CellEventArgs e) {#handleCellEvent-java.lang.Object-com.aspose.gridweb.CellEventArgs-}
```
public abstract String handleCellEvent(Object sender, CellEventArgs e)
```


manejar el evento de celda relacionado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | java.lang.Object | La cuadrícula de origen del evento. |
| e | [CellEventArgs](../../com.aspose.gridweb/celleventargs) | El argumento del evento. e.Cell es la celda que dispara el evento. e.Argument contiene el argumento del evento. |

**Returns:**
java.lang.String - valor de cadena
