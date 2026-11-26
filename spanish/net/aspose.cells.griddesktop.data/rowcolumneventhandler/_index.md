---
title: "Delegate RowColumnEventHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Representa la interfaz que pretende manejar eventos de fila/columna"
type: docs
url: /es/net/aspose.cells.griddesktop.data/rowcolumneventhandler/
---
## RowColumnEventHandler delegate

Representa la interfaz que pretende manejar eventos de fila/columna.

void **handleCellEvent**(Object sender, RowColumnEventArgs e);

```csharp
public delegate void RowColumnEventHandler(object sender, RowColumnEventArgs e);
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | Objeto | El origen del evento. |
| e | RowColumnEventArgs | El argumento del evento. Llame a e.RejectOperation() si desea cancelar la operación de eliminación en los controladores de eventos RowDeleting o ColumnDeleting. |

### Ver también

* class [RowColumnEventArgs](../../aspose.cells.griddesktop/rowcolumneventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


