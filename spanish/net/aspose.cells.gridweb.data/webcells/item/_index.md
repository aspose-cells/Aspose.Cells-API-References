---
title: "WebCells.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WebCells. Obtiene el elemento Cell en el índice de fila y columna de celda especificados"
type: docs
url: /es/net/aspose.cells.gridweb.data/webcells/item/
---
## WebCells indexer (1 of 2)

Obtiene el elemento Cell en el índice de fila y columna de celda especificados.

```csharp
public WebCell this[int row, int column] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| fila | Índice de fila. |
| columna | Índice de columna. |

### Valor de retorno

El objeto Cell.

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

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## WebCells indexer (2 of 2)

Obtiene el elemento Cell con el nombre de celda especificado.

```csharp
public WebCell this[string cellName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| cellName | Nombre de la celda, incluyendo su letra de columna y número de fila, por ejemplo A5. |

### Valor de retorno

Un objeto Cell

### Ejemplos

```csharp
[C#]

Cells cells = excel.Worksheets[0].Cells;
Cell cell = cells["A1"];	//Gets the cell at "A1"

[Visual Basic]

Dim cells As Cells =  excel.Worksheets(0).Cells
Dim cell As Cell =  cells("A1")  'Gets the cell at "A1"
```

### Ver también

* class [WebCell](../../webcell/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


