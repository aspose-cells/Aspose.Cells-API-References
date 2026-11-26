---
title: "Cells.SetColumnWidthPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Establece el ancho de columna en unidades de píxeles en vista normal"
type: docs
url: /es/net/aspose.cells/cells/setcolumnwidthpixel/
---
## Cells.SetColumnWidthPixel method

Establece el ancho de la columna en unidades de píxeles en vista normal.

```csharp
public void SetColumnWidthPixel(int column, int pixels)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |
| píxeles | Int32 | Número de píxeles. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establece el ancho de columnas en píxeles para las columnas 1 a 5
            for (int i = 0; i < 5; i++)
            {
                cells.SetColumnWidthPixel(i, 120); // 120 pixels width
            }

            // Guarda el libro de trabajo
            workbook.Save("SetColumnWidthPixelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


