---
title: "Cells.SetViewColumnWidthPixel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Establece el ancho de la columna en diferentes vistas"
type: docs
url: /es/net/aspose.cells/cells/setviewcolumnwidthpixel/
---
## Cells.SetViewColumnWidthPixel method

Establece el ancho de la columna en diferentes vistas.

```csharp
public void SetViewColumnWidthPixel(int column, int pixels)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | El índice de columna. |
| píxeles | Int32 | El ancho en unidades de píxeles. |

### Observaciones

Si el tipo de vista actual es PageLayoutView, el ancho de la columna es el mismo que el ancho impreso.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetViewColumnWidthPixelWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Establecer datos de muestra
            sheet.Cells[0, 0].Value = "Sample Text";

            // Calcular el ancho en píxeles (100 píxeles en este ejemplo)
            int pixelWidth = 100;

            // Establecer el ancho de la columna en píxeles
            sheet.Cells.SetViewColumnWidthPixel(0, pixelWidth);

            // Guarda el libro de trabajo
            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


