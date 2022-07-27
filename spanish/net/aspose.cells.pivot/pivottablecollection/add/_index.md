---
title: Add
second_title: Referencia de API de Aspose.Cells para .NET
description: Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.
type: docs
weight: 20
url: /es/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string, string) {#add_4}

Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceData | String | Los datos para la nueva caché de tabla dinámica. |
| destCellName | String | La celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe de tabla dinámica. |

### Valor_devuelto

El nuevo índice de caché agregado.

### Ver también

* class [PivotTableCollection](../../pivottablecollection)
* espacio de nombres [Aspose.Cells.Pivot](../../pivottablecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_5}

Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceData | String | Los datos para la nueva caché de tabla dinámica. |
| destCellName | String | La celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe de tabla dinámica. |
| useSameSource | Boolean | Indica si se usa la misma fuente de datos cuando otra tabla dinámica existente ha usado esta fuente de datos. Si la propiedad es verdadera, ahorrará memoria. |

### Valor_devuelto

El nuevo índice de caché agregado.

### Ver también

* class [PivotTableCollection](../../pivottablecollection)
* espacio de nombres [Aspose.Cells.Pivot](../../pivottablecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_2}

Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.

```csharp
public int Add(string sourceData, int row, int column, string tableName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva tabla dinámica. Ejemplo: Sheet1! A1: C8 |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe de tabla dinámica. |

### Valor_devuelto

El nuevo índice de caché agregado.

### Ver también

* class [PivotTableCollection](../../pivottablecollection)
* espacio de nombres [Aspose.Cells.Pivot](../../pivottablecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_3}

Agrega una nueva caché de tabla dinámica a una colección de PivotCaches.

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceData | String | El rango de celdas de datos para la nueva tabla dinámica. Ejemplo: Sheet1! A1: C8 |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe de tabla dinámica. |
| useSameSource | Boolean | Indica si se usa la misma fuente de datos cuando otra tabla dinámica existente ha usado esta fuente de datos. Si la propiedad es verdadera, ahorrará memoria. |

### Valor_devuelto

El nuevo índice de caché agregado.

### Ver también

* class [PivotTableCollection](../../pivottablecollection)
* espacio de nombres [Aspose.Cells.Pivot](../../pivottablecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_1}

Agrega un nuevo objeto de tabla dinámica a la colección desde otra tabla dinámica.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivotTable | PivotTable | La tabla dinámica de origen. |
| destCellName | String | La celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe de tabla dinámica. |

### Valor_devuelto

El nuevo índice de tabla dinámica agregado.

### Ver también

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* espacio de nombres [Aspose.Cells.Pivot](../../pivottablecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add}

Agrega un nuevo objeto de tabla dinámica a la colección desde otra tabla dinámica.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pivotTable | PivotTable | La tabla dinámica de origen. |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe de tabla dinámica. |

### Valor_devuelto

El nuevo índice de tabla dinámica agregado.

### Ver también

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* espacio de nombres [Aspose.Cells.Pivot](../../pivottablecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_7}

Agrega un nuevo objeto de tabla dinámica a la colección con varios rangos de consolidación como origen de datos.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceData | String[] | Los múltiples rangos de consolidación, como {"Hoja1!A1:C8","Hoja2!A1:B8"} |
| isAutoPage | Boolean | Si se crea automáticamente un campo de una sola página. Si es verdadero, se ignorarán los siguientes parámetros pageFields. |
| pageFields | PivotPageFields | El campo de la página dinámica items. |
| destCellName | String | destCellName El nombre del nuevo informe de tabla dinámica. |
| tableName | String | el nombre del nuevo informe de tabla dinámica. |

### Valor_devuelto

El nuevo índice de tabla dinámica agregado.

### Ver también

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* espacio de nombres [Aspose.Cells.Pivot](../../pivottablecollection)
* asamblea [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_6}

Agrega un nuevo objeto de tabla dinámica a la colección con varios rangos de consolidación como origen de datos.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| sourceData | String[] | Los múltiples rangos de consolidación, como {"Hoja1!A1:C8","Hoja2!A1:B8"} |
| isAutoPage | Boolean | Si se crea automáticamente un campo de una sola página. Si es verdadero, se ignorarán los siguientes parámetros pageFields |
| pageFields | PivotPageFields | El campo de la página dinámica items. |
| row | Int32 | Índice de fila de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| column | Int32 | Índice de columna de la celda en la esquina superior izquierda del rango de destino del informe de tabla dinámica. |
| tableName | String | El nombre del nuevo informe de tabla dinámica. |

### Valor_devuelto

El nuevo índice de tabla dinámica agregado.

### Ver también

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* espacio de nombres [Aspose.Cells.Pivot](../../pivottablecollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
