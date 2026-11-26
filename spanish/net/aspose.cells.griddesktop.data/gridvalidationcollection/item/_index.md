---
title: "GridValidationCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GridValidationCollection. Obtiene el elemento Hyperlink en el índice especificado."
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridvalidationcollection/item/
---
## GridValidationCollection indexer (1 of 2)

Obtiene el elemento de hipervínculo en el índice especificado.

```csharp
public GridValidation this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ver también

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## GridValidationCollection indexer (2 of 2)

Obtiene el elemento [`GridValidation`](../../gridvalidation/) en la celda especificada. Si no hay validación, devuelve null.

```csharp
public GridValidation this[int row, int column] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| fila | La fila de la celda. |
| columna | La columna de la celda. |

### Valor de retorno

El elemento en el índice especificado.

### Observaciones

Si no hay un objeto de validación en el índice de fila y columna especificado, esto comprobará el objeto de validación de la columna.

### Ver también

* class [GridValidation](../../gridvalidation/)
* class [GridValidationCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


