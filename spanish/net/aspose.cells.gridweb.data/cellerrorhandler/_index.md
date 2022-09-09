---
title: CellErrorHandler
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa la interfaz que pretende manejar eventos de error de celda.
type: docs
weight: 80
url: /es/net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

Representa la interfaz que pretende manejar eventos de error de celda.

vacío **manejarCellEvent**(Remitente del objeto, GridCellException ex, consulta OnErrorActionQuery);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sender | Object | La fuente del evento. |
| ex | WebCellException | El error de operación de la celda. |
| action | OnErrorActionQuery | puede obtener información sobre el tipo de acción onerror. |

### Ver también

* class [WebCellException](../webcellexception)
* class [OnErrorActionQuery](../onerroractionquery)
* espacio de nombres [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* asamblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->