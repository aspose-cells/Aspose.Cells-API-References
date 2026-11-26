---
title: "Delegado CellErrorHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Representa la interfaz que pretende manejar eventos de error de celda"
type: docs
url: /es/net/aspose.cells.gridweb.data/cellerrorhandler/
---
## CellErrorHandler delegate

Representa la interfaz que pretende manejar eventos de error de celda.

void **handleCellEvent**(Object sender, GridCellException ex, OnErrorActionQuery query);

```csharp
public delegate void CellErrorHandler(object sender, WebCellException ex, 
    OnErrorActionQuery action);
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | Objeto | El origen del evento. |
| ex | WebCellException | El error de operación de la celda. |
| acción | OnErrorActionQuery | puede obtener información del tipo de acción onerror. |

### Ver también

* class [WebCellException](../webcellexception/)
* class [OnErrorActionQuery](../onerroractionquery/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


