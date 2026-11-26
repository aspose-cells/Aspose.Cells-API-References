---
title: "WebWorksheet.CreateSubtotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "WebWorksheet método. Crea un subtotal en la hoja"
type: docs
url: /es/net/aspose.cells.gridweb.data/webworksheet/createsubtotal/
---
## WebWorksheet.CreateSubtotal method

Crea un subtotal en la hoja.

```csharp
public void CreateSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, 
    SubtotalFunction subtotalFunction, int[] subtotalColumnIndexList, string functionLabel, 
    GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, NumberType numberType, 
    string customString)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columnNameRowIndex | Int32 | El índice de fila de la fila de nombre de columna. |
| dataRows | Int32 | El número de filas de datos. |
| groupByColumnIndex | Int32 | El índice de columna de la columna a agrupar. |
| subtotalFunction | SubtotalFunction | El tipo de función de subtotal. |
| subtotalColumnIndexList | Int32[] | Los índices de columna a subtotalizar. |
| functionLabel | String | La etiqueta de la función de subtotal. |
| grandCellStyle | GridTableItemStyle | El estilo de la línea de total general. |
| subtotalCellStyle | GridTableItemStyle | El estilo de la línea de subtotal. |
| numberType | NumberType | El tipo numérico de las celdas de resultados de subtotal. |
| customString | String | La cadena de formato personalizada de las celdas de resultados de subtotal. Puede ser nula. |

### Ver también

* enum [SubtotalFunction](../../subtotalfunction/)
* class [GridTableItemStyle](../../../aspose.cells.gridweb/gridtableitemstyle/)
* enum [NumberType](../../numbertype/)
* class [WebWorksheet](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


