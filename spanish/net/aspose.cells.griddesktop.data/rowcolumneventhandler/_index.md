---
title: RowColumnEventHandler
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa la interfaz que pretende manejar eventos de fila/columna.
type: docs
weight: 780
url: /es/net/aspose.cells.griddesktop.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

Representa la interfaz que pretende manejar eventos de fila/columna.

vacío **manejarCellEvent**(Remitente del objeto, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sender | Object | La fuente del evento. |
| e | RowColumnEventArgs | El argumento del evento. Llame a e.RejectOperation() si desea cancelar la operación de eliminación en los controladores de eventos RowDeleting o ColumnDeleting. |

### Ver también

* class [RowColumnEventArgs](../../aspose.cells.griddesktop/rowcolumneventargs)
* espacio de nombres [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* asamblea [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->