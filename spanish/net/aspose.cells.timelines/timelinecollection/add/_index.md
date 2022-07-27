---
title: Add
second_title: Referencia de API de Aspose.Cells para .NET
description: Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos
type: docs
weight: 20
url: /es/net/aspose.cells.timelines/timelinecollection/add/
---
## Add(PivotTable, int, int, string) {#add_2}

Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de la línea de tiempo. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de la línea de tiempo. |
| baseFieldName | String | El nombre de PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice de línea de tiempo agregado

### Ejemplos

```csharp

[C#]
//Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos
sheet.Timelines.Add(pivot, 10, 5, "date");
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* espacio de nombres [Aspose.Cells.Timelines](../../timelinecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_5}

Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| destCellName | String | El nombre de la celda en la esquina superior izquierda del rango de la línea de tiempo. |
| baseFieldName | String | El nombre de PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice de línea de tiempo agregado

### Ejemplos

```csharp

[C#]
//Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos
sheet.Timelines.Add(pivot, "i15", "date");
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* espacio de nombres [Aspose.Cells.Timelines](../../timelinecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de la línea de tiempo. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de la línea de tiempo. |
| baseFieldIndex | Int32 | El índice de PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice de línea de tiempo agregado

### Ejemplos

```csharp

[C#]
//Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos
sheet.Timelines.Add(pivot, 15, 5, 1);
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* espacio de nombres [Aspose.Cells.Timelines](../../timelinecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| destCellName | String | El nombre de la celda en la esquina superior izquierda del rango de la línea de tiempo. |
| baseFieldIndex | Int32 | El índice de PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice de línea de tiempo agregado

### Ejemplos

```csharp

[C#]
//Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos
sheet.Timelines.Add(pivot, "i5", 1);
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [TimelineCollection](../../timelinecollection)
* espacio de nombres [Aspose.Cells.Timelines](../../timelinecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de la línea de tiempo. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de la línea de tiempo. |
| baseField | PivotField | El PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice de línea de tiempo agregado

### Ejemplos

```csharp

[C#]
//Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* espacio de nombres [Aspose.Cells.Timelines](../../timelinecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| destCellName | String | El nombre de la celda en la esquina superior izquierda del rango de la línea de tiempo. |
| baseField | PivotField | El PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice de línea de tiempo agregado

### Ejemplos

```csharp

[C#]
//Agregue una nueva línea de tiempo usando una tabla dinámica como fuente de datos
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[1]);
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [TimelineCollection](../../timelinecollection)
* espacio de nombres [Aspose.Cells.Timelines](../../timelinecollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
