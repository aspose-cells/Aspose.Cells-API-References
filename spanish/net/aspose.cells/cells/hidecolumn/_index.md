---
title: "Cells.HideColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Oculta una columna"
type: docs
url: /es/net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

Oculta una columna.

```csharp
public void HideColumn(int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer algunos datos en la columna que ocultaremos
            cells["B1"].PutValue("This column will be hidden");
            cells["B2"].PutValue(123.45);

            // Ocultar la columna B (índice 1)
            cells.HideColumn(1);

            // Mostrar la columna con ancho estándar
            cells.UnhideColumn(1, cells.StandardWidth);

            // Guarda el libro de trabajo
            workbook.Save("HideColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


