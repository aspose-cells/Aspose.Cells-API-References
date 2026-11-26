---
title: "Enum GridRenameStrategy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.GridDesktop.Data.GridRenameStrategy enum. Opción de estrategia para nombres duplicados de columnas"
type: docs
url: /es/net/aspose.cells.griddesktop.data/gridrenamestrategy/
---
## GridRenameStrategy enumeration

Opción de estrategia para nombres duplicados de columnas.

```csharp
public enum GridRenameStrategy
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Exception | `0` | Lanza una excepción. |
| Digit | `1` | Nombrado con dígito. Los nombres duplicados se convertirán en ...1, ...2, etc. |
| Letter | `2` | Nombrado con letra.. Los nombres duplicados se convertirán en ...A, ...B, etc. |

### Observaciones

Al procesar datos con encabezados, algunos escenarios requieren que los encabezados no se dupliquen en ninguna columna. Por ejemplo, al exportar datos a una DataTable y que el encabezado deba tomarse como el nombre de columna de la DataTable, los valores duplicados del encabezado son inválidos. Para este tipo de situaciones, el usuario puede determinar cómo manejarlos especificando esta estrategia.

### Ver también

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


