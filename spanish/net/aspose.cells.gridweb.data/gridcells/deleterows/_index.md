---
title: "GridCells.DeleteRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "GridCells método. Elimina varias filas"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridcells/deleterows/
---
## DeleteRows(int, int) {#deleterows}

Elimina varias filas.

```csharp
public bool DeleteRows(int rowIndex, int totalRows)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | El índice de la primera fila a eliminar. |
| totalRows | Int32 | Número de filas a eliminar. |

### Observaciones

Si el rango eliminado contiene la parte superior (no completa) de la tabla (ListObject), el rango no podrá ser eliminado y no se hará nada.Funciona como MS Excel.

### Ver también

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## DeleteRows(int, int, bool) {#deleterows_1}

Elimina varias filas en la hoja de cálculo.

```csharp
public bool DeleteRows(int rowIndex, int totalRows, bool updateReference)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | Índice de fila. |
| totalRows | Int32 | Número de filas a eliminar. |
| updateReference | Booleano | Indica si actualizar referencias en otras hojas de cálculo. |

### Ver también

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


