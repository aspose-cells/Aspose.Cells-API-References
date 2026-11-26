---
title: "WebCells.Export"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WebCells. Exporta los datos de la colección Cells de un WebWorksheet a un nuevo objeto DataTable."
type: docs
url: /es/net/aspose.cells.gridweb.data/webcells/export/
---
## WebCells.Export method

Exporta datos de la colección Cells de un WebWorksheet a un nuevo objeto DataTable

```csharp
public DataTable Export(int startRow, int startColumn, int rows, int columns, 
    bool exportColumnName, bool isVertical)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | El número de fila de la primera celda a exportar. |
| startColumn | Int32 | El número de columna de la primera celda a exportar. |
| filas | Int32 | Número de filas a importar. |
| columnas | Int32 | Número de columnas a importar. |
| exportColumnName | Booleano | Indica si los datos en la primera fila se exportan como el nombre de columna del DataTable. |
| isVertical | Booleano | True si una fila en el archivo Excel representa una fila en el DataTable. False si una columna en el archivo Excel representa una fila en el DataTable. |

### Valor de retorno

Objeto DataTable exportado.

### Ver también

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


