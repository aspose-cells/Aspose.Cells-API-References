---
title: "Delegado CellEventStringHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Representa el método que pretende manejar eventos de celda. Igual que la interfaz CellEventHandler pero devuelve un resultado de tipo cadena"
type: docs
url: /es/net/aspose.cells.gridweb.data/celleventstringhandler/
---
## CellEventStringHandler delegate

Representa el método que pretende manejar eventos de celda. igual que la interfaz CellEventHandler, pero devuelve un resultado de cadena

String **handleCellEvent**(Object sender, CellEventArgs e);

```csharp
public delegate string CellEventStringHandler(object sender, CellEventArgs e);
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| remitente | Objeto | La cuadrícula origen del evento. |
| e | CellEventArgs | El argumento del evento. e.Cell es la celda que dispara el evento. e.Argument contiene el argumento del evento. |

### Valor de retorno

string valor

### Ver también

* class [CellEventArgs](../../aspose.cells.gridweb/celleventargs/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


