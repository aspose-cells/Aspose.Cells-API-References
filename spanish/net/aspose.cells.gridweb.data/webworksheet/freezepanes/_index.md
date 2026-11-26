---
title: "WebWorksheet.FreezePanes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "WebWorksheet método. Congela los paneles en la celda especificada de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.gridweb.data/webworksheet/freezepanes/
---
## WebWorksheet.FreezePanes method

Congela paneles en la celda especificada de la hoja de cálculo.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |
| columna | Int32 | Índice de columna. |
| freezedRows | Int32 | Número de filas visibles en el panel superior, no más que el índice de fila. |
| freezedColumns | Int32 | Número de columnas visibles en el panel izquierdo, no más que el índice de columna. |

### Observaciones

El índice de fila y el índice de columna no pueden ser ambos cero. El número de filas y el número de columnas tampoco pueden ser ambos cero.

Los dos primeros parámetros especifican la posición congelada y los dos últimos parámetros especifican el área congelada en el panel superior izquierdo.

### Ver también

* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


