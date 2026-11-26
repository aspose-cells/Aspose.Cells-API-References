---
title: "GridCells.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GridCells. Obtiene el elemento GridCell en el índice de fila y columna de celda especificados"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridcells/item/
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
GridWeb GridWeb1 = new GridWeb();
GridCells cells = GridWeb1.WorkSheets[0].Cells;
//Obtiene la celda en "A1"
GridCell cell = cells[0, 0];	

[Visual Basic]

Dim cells As Cells =  excel.WorkSheets(0).Cells
 'Gets the cell at "A1"
Dim cell As Cell =  cells(0,0) 
```

### Ver también

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

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

### Ejemplos

```csharp
[C#]
ridWeb GridWeb1 = new GridWeb();
 GridCells cells = GridWeb1.WorkSheets[0].Cells;
 GridCell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Ver también

* class [GridCell](../../gridcell/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


