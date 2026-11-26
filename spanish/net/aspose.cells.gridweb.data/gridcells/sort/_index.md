---
title: "GridCells.Sort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridCells. Ordena los datos de forma ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo según el índice de columna especificado. Ordena los datos de forma ascendente/descendente de izquierda a derecha en un rango de una hoja de cálculo según el índice de fila especificado."
type: docs
url: /es/net/aspose.cells.gridweb.data/gridcells/sort/
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
 GridWeb GridWeb1 = new GridWeb();
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Ver también

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_1}

Ordena los datos ascendente/descendente de arriba a abajo en un rango de una hoja de cálculo por el índice de columna especificado. Ordena los datos ascendente/descendente de izquierda a derecha en un rango de una hoja de cálculo por el índice de fila especificado.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | El número de fila de la primera celda a ordenar. |
| startColumn | Int32 | El número de columna de la primera celda a ordenar. |
| filas | Int32 | Número de filas a importar. |
| columnas | Int32 | Número de columnas a importar. |
| índices | Int32[] | La matriz de índices de columna que especifica la columna de ordenación. Si la Orientación es de arriba a abajo, representa el índice de columna que especifica la columna de ordenación. Si la Orientación es de izquierda a derecha, representa el índice de fila que especifica la fila de ordenación. |
| órdenes | SortByOrder[] | la matriz de orden de clasificación. |
| orientación | SortOrientation | orientación de ordenación |
| isCaseSensitive | Booleano | si la ordenación distingue entre mayúsculas y minúsculas. |

### Ejemplos

```csharp

 [C#]
 GridWeb GridWeb1=new GridWeb();
 int[] ids={0,1};
 SortByOrder[] sorder={SortByOrder.Ascending,SortByOrder.Descending};
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false);

 [VB]

 GridWeb1.WorkSheets(0).Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false)

```

### Ver también

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


