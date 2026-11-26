---
title: "Delegate RowColumnEventHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Representa la interfaz que pretende manejar eventos de fila/columna"
type: docs
url: /es/net/aspose.cells.gridweb.data/rowcolumneventhandler/
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

* class [RowColumnEventArgs](../../aspose.cells.gridweb/rowcolumneventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


