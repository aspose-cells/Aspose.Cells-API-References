---
title: "GridValidation.GetListValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridValidation. Obtiene el valor de la lista de validación para la celda especificada."
type: docs
url: /es/net/aspose.cells.gridweb.data/gridvalidation/getlistvalue/
---
## GridValidation.GetListValue method

Obtenga el valor de la lista de validación para la celda especificada.

```csharp
public object GetListValue(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | El índice de columna. |

### Valor de retorno

El valor para generar la lista de esta validación para la celda especificada. Si la lista hace referencia a un rango, el valor devuelto será un objeto ReferredArea; de lo contrario, el valor devuelto puede ser null, object[] o un objeto simple.

### Observaciones

Solo para validaciones cuyo tipo es List y que se han aplicado a la celda dada; de lo contrario se devolverá null.

### Ver también

* class [GridValidation](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


