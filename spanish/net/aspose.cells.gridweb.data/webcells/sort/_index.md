---
title: "WebCells.Sort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WebCells. Ordena los datos de forma ascendente de arriba a abajo en un rango de un WebWorksheet por el índice de columna especificado"
type: docs
url: /es/net/aspose.cells.gridweb.data/webcells/sort/
---
## Sort(int, int, int, int, int) {#sort}

Ordena los datos de forma ascendente de arriba a abajo en un rango de un WebWorksheet por el índice de columna especificado.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | El número de fila de la primera celda a ordenar. |
| startColumn | Int32 | El número de columna de la primera celda a ordenar. |
| filas | Int32 | Número de filas a importar. |
| columnas | Int32 | Número de columnas a importar. |
| índice | Int32 | El índice de columna que especifica la columna de ordenamiento. |

### Ejemplos

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)

```

### Ver también

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}

Ordena los datos de forma ascendente de arriba a abajo en un rango de un WebWorksheet por el índice de columna especificado.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, 
    SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | El número de fila de la primera celda a ordenar. |
| startColumn | Int32 | El número de columna de la primera celda a ordenar. |
| filas | Int32 | Número de filas a importar. |
| columnas | Int32 | Número de columnas a importar. |
| índice | Int32 | El índice de columna (o fila) que especifica la columna (o fila) de ordenamiento. Si la orientación del ordenamiento es de arriba a abajo, el índice representa el índice de columna. Si la orientación del ordenamiento es de izquierda a derecha, el índice representa el índice de fila. |
| orden | SortByOrder | El orden de clasificación: Ascendente o Descendente |
| orientación | SortOrientation | La orientación del ordenamiento: de arriba a abajo o de izquierda a derecha. |
| isCaseSensitive | Booleano | Indica si los datos de ordenamiento distinguen mayúsculas y minúsculas cuando los datos son una cadena. |

### Ejemplos

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)

```

### Ver también

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[]) {#sort_2}

Ordena los datos de forma ascendente de arriba a abajo en un rango de un WebWorksheet por algunos campos especificados mediante una matriz de índices de columnas.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | El número de fila de la primera celda a ordenar. |
| startColumn | Int32 | El número de columna de la primera celda a ordenar. |
| filas | Int32 | Número de filas a importar. |
| columnas | Int32 | Número de columnas a importar. |
| índices | Int32[] | La matriz de índices de columna que especifica los datos por los que se ordena. |

### Ejemplos

```csharp

[C#]

int[] indexes = new int[3];
indexes[0] = 0;
indexes[1] = 2;
indexes[2] = 3;
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,indexes);

[VB]

Dim indexes() As Integer =  New Integer(3) {} 
indexes(0) = 0
indexes(1) = 2
indexes(2) = 3
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,indexes)

```

### Ver también

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}

Ordena los datos de forma ascendente en un rango de un WebWorksheet por algunos campos especificados mediante una matriz de índices.

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
| índices | Int32[] | El índice de columna (o fila) que especifica la columna (o fila) de ordenamiento. Si la orientación del ordenamiento es de arriba a abajo, el índice representa el índice de columna. Si la orientación del ordenamiento es de izquierda a derecha, el índice representa el índice de fila. |
| órdenes | SortByOrder[] | El orden de clasificación: Ascendente o Descendente |
| orientación | SortOrientation | La orientación del ordenamiento: de arriba a abajo o de izquierda a derecha. |
| isCaseSensitive | Booleano | Indica si el ordenamiento distingue mayúsculas y minúsculas. |

### Observaciones

Si utiliza este método para ordenar un bloque de datos, asegúrese de que la longitud del parámetro índices sea igual a la longitud del parámetro órdenes.

### Ejemplos

```csharp

```

[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)

### Ver también

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


