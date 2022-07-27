---
title: Add
second_title: Referencia de API de Aspose.Cells para .NET
description: Agregue una nueva segmentación usando la tabla dinámica como fuente de datos
type: docs
weight: 20
url: /es/net/aspose.cells.slicers/slicercollection/add/
---
## Add(PivotTable, string, string) {#add_5}

Agregue una nueva segmentación usando la tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| destCellName | String | La celda en la esquina superior izquierda del rango Slicer. |
| baseFieldName | String | El nombre de PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice Add Slicer

### Ejemplos

```csharp

[C#]

slicers.Add(pivot, "E3", "fruit");
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* espacio de nombres [Aspose.Cells.Slicers](../../slicercollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add_2}

Agregue una nueva segmentación usando la tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de Slicer. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de Slicer. |
| baseFieldName | String | El nombre de PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice Add Slicer

### Ejemplos

```csharp

[C#]

slicers.Add(pivot, 20, 12, "fruit");
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* espacio de nombres [Aspose.Cells.Slicers](../../slicercollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, int) {#add_1}

Agregue una nueva segmentación usando la tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de Slicer. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de Slicer. |
| baseFieldIndex | Int32 | El índice de PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice Add Slicer

### Ejemplos

```csharp

[C#]

slicers.Add(pivot, 20, 8, 0);
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* espacio de nombres [Aspose.Cells.Slicers](../../slicercollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, int) {#add_4}

Agregue una nueva segmentación usando la tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| destCellName | String | La celda en la esquina superior izquierda del rango Slicer. |
| baseFieldIndex | Int32 | El índice de PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice Add Slicer

### Ejemplos

```csharp

[C#]

slicers.Add(pivot, "E20", 0);
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [SlicerCollection](../../slicercollection)
* espacio de nombres [Aspose.Cells.Slicers](../../slicercollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, PivotField) {#add}

Agregue una nueva segmentación usando la tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de Slicer. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de Slicer. |
| baseField | PivotField | El PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice Add Slicer

### Ejemplos

```csharp

[C#]

slicers.Add(pivot, 3, 12, pivot.BaseFields[0]);
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* espacio de nombres [Aspose.Cells.Slicers](../../slicercollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, PivotField) {#add_3}

Agregue una nueva segmentación usando la tabla dinámica como fuente de datos

```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivot | PivotTable | Objeto de tabla dinámica |
| destCellName | String | La celda en la esquina superior izquierda del rango Slicer. |
| baseField | PivotField | El PivotField en PivotTable.BaseFields |

### Valor_devuelto

El nuevo índice Add Slicer

### Ejemplos

```csharp

[C#]

slicers.Add(pivot, "I3", pivot.BaseFields[0]);
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable)
* class [PivotField](../../../aspose.cells.pivot/pivotfield)
* class [SlicerCollection](../../slicercollection)
* espacio de nombres [Aspose.Cells.Slicers](../../slicercollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(ListObject, int, string) {#add_8}

Agregue un nuevo Slicer usando ListObjet como fuente de datos

```csharp
public int Add(ListObject table, int index, string destCellName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| table | ListObject | objeto ListObject |
| index | Int32 | El índice de ListColumn en ListObject.ListColumns |
| destCellName | String | La celda en la esquina superior izquierda del rango Slicer. |

### Valor_devuelto

El nuevo índice Add Slicer

### Ejemplos

```csharp

[C#]

slicers.Add(table, 1, "E38");
```

### Ver también

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [SlicerCollection](../../slicercollection)
* espacio de nombres [Aspose.Cells.Slicers](../../slicercollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, string) {#add_7}

Agregue un nuevo Slicer usando ListObjet como fuente de datos

```csharp
public int Add(ListObject table, ListColumn listColumn, string destCellName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| table | ListObject | objeto ListObject |
| listColumn | ListColumn | ListColumn en ListObject.ListColumns |
| destCellName | String | La celda en la esquina superior izquierda del rango Slicer. |

### Valor_devuelto

El nuevo índice Add Slicer

### Ejemplos

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], "I38");
```

### Ver también

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* espacio de nombres [Aspose.Cells.Slicers](../../slicercollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(ListObject, ListColumn, int, int) {#add_6}

Agregue un nuevo Slicer usando ListObjet como fuente de datos

```csharp
public int Add(ListObject table, ListColumn listColumn, int row, int column)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| table | ListObject | objeto ListObject |
| listColumn | ListColumn | ListColumn en ListObject.ListColumns |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de Slicer. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de Slicer. |

### Valor_devuelto

El nuevo índice Add Slicer

### Ejemplos

```csharp

[C#]

slicers.Add(table, table.ListColumns[1], 38, 12);
```

### Ver también

* class [ListObject](../../../aspose.cells.tables/listobject)
* class [ListColumn](../../../aspose.cells.tables/listcolumn)
* class [SlicerCollection](../../slicercollection)
* espacio de nombres [Aspose.Cells.Slicers](../../slicercollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
