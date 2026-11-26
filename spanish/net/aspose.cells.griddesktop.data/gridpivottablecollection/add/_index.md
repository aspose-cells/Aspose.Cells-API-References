---
title: "GridPivotTableCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridPivotTableCollection. Agrega una nueva caché de PivotTable a una colección PivotCaches"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridpivottablecollection/add/
---
## Add(string, string, string) {#add_3}

Añade una nueva caché de PivotTable a una colección PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva PivotTable. Ejemplo: Sheet1!A1:C8 |
| destCellName | String | La celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| tableName | String | El nombre del nuevo informe PivotTable. |

### Valor de retorno

El índice de la caché recién añadida.

### Ver también

* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(Worksheet, GridCellArea, string, string) {#add}

Añade una nueva caché de PivotTable a una colección PivotCaches.

```csharp
public int Add(Worksheet sourceSheet, GridCellArea sourceArea, string destCellName, 
    string tableName)
```

| Parámetro | Descripción |
| --- | --- |
| sourceSheet | La hoja de cálculo fuente. |
| sourceArea | El área en la hoja de cálculo fuente. |
| destRow | La fila de la celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| destCol | La columna de la celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| tableName | El nombre del nuevo informe PivotTable. |

### Valor de retorno

El índice de la caché recién añadida.

### Ver también

* class [Worksheet](../../../aspose.cells.griddesktop/worksheet/)
* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, int, int, string) {#add_1}

Añade una nueva caché de PivotTable a una colección PivotCaches.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, int destRow, int destCol, 
    string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| worksheetname | String | El nombre de la hoja de cálculo fuente. |
| sourceArea | GridCellArea | El área en la hoja de cálculo fuente. |
| destRow | Int32 | La fila de la celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| destCol | Int32 | La columna de la celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| tableName | String | El nombre del nuevo informe PivotTable. |

### Valor de retorno

El índice de la caché recién añadida.

### Ver también

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, string, string) {#add_2}

Añade una nueva caché de PivotTable a una colección PivotCaches.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, string destCellName, string tableName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| worksheetname | String | El nombre de la hoja de cálculo fuente. |
| sourceArea | GridCellArea | El área en la hoja de cálculo fuente. |
| destCellName | String | La celda en la esquina superior izquierda del rango de destino del informe PivotTable. |
| tableName | String | El nombre del nuevo informe PivotTable. |

### Valor de retorno

El índice de la caché recién añadida.

### Ver también

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


