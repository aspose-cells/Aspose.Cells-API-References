---
title: "Cells.SetRowHeightPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Establece la altura de la fila en unidades de píxeles"
type: docs
url: /es/net/aspose.cells/cells/setrowheightpixel/
---
## Cells.SetRowHeightPixel method

Establece la altura de la fila en unidades de píxeles.

```csharp
public void SetRowHeightPixel(int row, int pixels)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila. |
| píxeles | Int32 | Número de píxeles. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establece la altura de la primera fila a 50 píxeles
            worksheet.Cells.SetRowHeightPixel(0, 50);

            // Establece la altura de la segunda fila a 100 píxeles
            worksheet.Cells.SetRowHeightPixel(1, 100);

            // Guarda el libro de trabajo
            workbook.Save("RowHeightPixelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


