---
title: "GridValidationCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridValidationCollection. Añade un GridValidation a la colección. La validación se aplica a la celda especificada."
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridvalidationcollection/add/
---
## Add(string) {#add_1}

Añade un [`GridValidation`](../../gridvalidation/) a la colección. La validación se aplica a la celda especificada.

```csharp
public GridValidation Add(string cellname)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellname | String | el nombre de la celda. |

### Valor de retorno

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Ver también

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int) {#add}

Añade un [`GridValidation`](../../gridvalidation/) a la colección. La validación se aplica a la celda especificada.

```csharp
public GridValidation Add(int row, int col)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda. |
| col | Int32 | Índice de columna de la celda. |

### Valor de retorno

[`GridValidation`](../../gridvalidation/) the added GridValidation instance.

### Ver también

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, bool, string) {#add_5}

Añade una validación a una celda especificada por nombre de celda.

```csharp
public void Add(string cellName, bool isRequired, string regEx)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda de la cuadrícula. |
| isRequired | Booleano | Valor que indica si el valor de la celda es obligatorio. |
| regEx | String | Expresión regular. |

### Ver también

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, ICustomValidation) {#add_2}

Añade una validación a una celda especificada en el índice de fila y columna.

```csharp
public void Add(int row, int col, ICustomValidation customValidation)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda. |
| col | Int32 | Índice de columna de la celda. |
| customValidation | ICustomValidation | Objeto de validación personalizada. |

### Ver también

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, bool, string) {#add_3}

Añade una validación a una celda especificada en el índice de fila y columna.

```csharp
public void Add(int row, int col, bool isRequired, string regEx)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda. |
| col | Int32 | Índice de columna de la celda. |
| isRequired | Booleano | Valor que indica si el valor de la celda es obligatorio. |
| regEx | String | Expresión regular. |

### Ver también

* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, ICustomValidation) {#add_4}

Añade una validación a una celda especificada por nombre de celda.

```csharp
public void Add(string cellName, ICustomValidation customValidation)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda de la cuadrícula. |
| customValidation | ICustomValidation | Objeto de validación personalizada. |

### Ver también

* interface [ICustomValidation](../../../aspose.cells.griddesktop/icustomvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


