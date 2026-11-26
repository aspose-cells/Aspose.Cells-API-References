---
title: "GridCells.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GridCells. Obtiene el elemento GridCell en el índice de fila y columna de celda especificados"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridcells/item/
---
## GridCells indexer (1 of 2)

Obtiene el elemento [`GridCell`](../../gridcell/) en el índice de fila y columna de celda especificados.

```csharp
public GridCell this[int row, int column] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| fila | Índice de fila. |
| columna | Índice de columna. |

### Valor de retorno

El objeto [`GridCell`](../../gridcell/).

### Ejemplos

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells[0, 0];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
Dim cell As Cell =  cells(0,0)  'Gets the cell at "A1"
```

### Ver también

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridCells indexer (2 of 2)

Obtiene el elemento [`GridCell`](../../gridcell/) con el nombre de celda especificado.

```csharp
public GridCell this[string cellName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| cellName | Nombre de la celda, incluyendo su letra de columna y número de fila, por ejemplo A5. |

### Valor de retorno

Un objeto [`GridCell`](../../gridcell/)

### Ver también

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


