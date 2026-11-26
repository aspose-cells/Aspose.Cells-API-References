---
title: "Delegado CellEventHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Representa la interfaz que tiene la intención de manejar eventos de celda"
type: docs
url: /es/net/aspose.cells.griddesktop.data/celleventhandler/
---
## CellEventHandler delegate

Representa la interfaz que pretende manejar eventos de celda.

void **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate void CellEventHandler(object sender, CellEventArgs e);
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | Objeto | La cuadrícula origen del evento. |
| e | CellEventArgs | El argumento del evento. e.Cell es la celda que dispara el evento. e.Argument contiene el argumento del evento. |

### Ver también

* class [CellEventArgs](../../aspose.cells.griddesktop/celleventargs/)
* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


