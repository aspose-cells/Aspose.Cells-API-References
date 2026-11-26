---
title: "CellControlCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellControlCollection. Obtiene el control de celda en el índice de fila y columna especificado."
type: docs
url: /es/net/aspose.cells.griddesktop/cellcontrolcollection/item/
---
## CellControlCollection indexer (1 of 2)

Obtiene el control de celda en el índice de fila y columna especificado.

```csharp
public CellControl this[int row, int col] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| fila | índice de fila. |
| col | índice de columna. |

### Observaciones

Si no hay un objeto CellControl en el índice de fila y columna especificado, esto verificará el objeto CellControl de la columna.

### Ver también

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## CellControlCollection indexer (2 of 2)

Obtiene el control de celda por el nombre de celda especificado.

```csharp
public CellControl this[string cellName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| cellName | nombre de celda (en formato de nombre de Excel, como 'A1', 'F22') |

### Observaciones

Si no hay un objeto CellControl en el índice de fila y columna especificado, esto verificará el objeto CellControl de la columna.

### Ver también

* class [CellControl](../../cellcontrol/)
* class [CellControlCollection](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


