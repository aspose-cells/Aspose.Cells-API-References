---
title: "Cells.SetColumnWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Establece el ancho de la columna especificada en vista normal"
type: docs
url: /es/net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

Establece el ancho de la columna especificada en vista normal.

```csharp
public void SetColumnWidth(int column, double width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |
| ancho | Double | Ancho de la columna en unidades de caracteres. El ancho de la columna debe estar entre 0 y 255. |

### Observaciones

Para la hoja de cálculo, el ancho de columna se mide como el número de caracteres del ancho máximo de dígito de los números 0~9 tal como se renderiza en la fuente del estilo normal.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 25.5);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


