---
title: CellEventStringHandler
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa el método que pretende manejar eventos de celda. igual que la interfaz CellEventHandler pero devuelve la cadena result
type: docs
weight: 100
url: /es/net/aspose.cells.gridweb.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Representa el método que pretende manejar eventos de celda. igual que la interfaz CellEventHandler, pero devuelve la cadena result

Cuerda **manejarCellEvent**(remitente del objeto, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sender | Object | La cuadrícula de origen del evento. |
| e | CellEventArgs | El argumento del evento. La e.Cell es la celda que dispara el evento. El e.Argument contiene el argumento del evento. |

### Valor_devuelto

valor de cadena

### Ver también

* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs)
* espacio de nombres [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* asamblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
