---
title: "Worksheet.FreezePanes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Worksheet. Congela paneles en la celda especificada de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.griddesktop/worksheet/freezepanes/
---
## FreezePanes(string, int, int) {#freezepanes_1}

Congela paneles en la celda especificada de la hoja de cálculo.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |
| freezedRows | Int32 | Número de filas visibles en el panel superior, no más que el índice de fila. |
| freezedColumns | Int32 | Número de columnas visibles en el panel izquierdo, no más que el índice de columna. |

### Observaciones

El índice de fila y el índice de columna no pueden ser ambos cero. El número de filas y el número de columnas tampoco pueden ser ambos cero.

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## FreezePanes(int, int, int, int) {#freezepanes}

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

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


