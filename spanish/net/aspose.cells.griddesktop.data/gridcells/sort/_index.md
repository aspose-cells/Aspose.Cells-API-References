---
title: "GridCells.Sort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridCells. Ordena los datos de forma ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo según el índice de columna especificado. Ordena los datos de forma ascendente/descendente de izquierda a derecha en un rango de una hoja de cálculo según el índice de fila especificado."
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

Ordena los datos ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo por el índice de columna especificado. Ordena los datos ascendente/descendente de izquierda a derecha en un rango de una hoja de cálculo por el índice de fila especificado.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | El número de fila de la primera celda a ordenar. |
| startColumn | Int32 | El número de columna de la primera celda a ordenar. |
| filas | Int32 | Número de filas a importar. |
| columnas | Int32 | Número de columnas a importar. |
| índice | Int32 | El índice de columna que especifica la columna de ordenación. Si la Orientación es de arriba a abajo, representa el índice de columna que especifica la columna de ordenación. Si la Orientación es de izquierda a derecha, representa el índice de fila que especifica la fila de ordenación. |
| isAsending | Booleano | si el orden de clasificación es ascendente. |
| isCaseSensitive | Booleano | si la ordenación distingue entre mayúsculas y minúsculas. |
| islefttoright | Booleano | si la orientación de la ordenación es de izquierda a derecha |

### Ejemplos

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Ver también

* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

Ordena los datos del área.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parámetro | Descripción |
| --- | --- |
| celdas | Las celdas contienen el área de datos. |
| startRow | La fila inicial del área. |
| startColumn | La columna inicial del área. |
| filas | el total de filas. |
| columnas | El total de columnas. |
| índices | El arreglo de índices de columna ordenados |
| órdenes | El arreglo de órdenes ordenados |
| orientación | la orientación de la ordenación: de izquierda a derecha o de arriba a abajo. |
| isCaseSensitive | si distingue entre mayúsculas y minúsculas al comparar cadenas.. |

### Ver también

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder/)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


