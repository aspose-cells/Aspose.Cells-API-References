---
title: "Cells.StandardHeightPixels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene o establece la altura predeterminada de la fila en esta hoja de cálculo en unidades de píxeles"
type: docs
url: /es/net/aspose.cells/cells/standardheightpixels/
---
## Cells.StandardHeightPixels property

Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de píxeles.

```csharp
public int StandardHeightPixels { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightPixelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer algunos datos en celdas
            cells["A1"].PutValue("Sample Data");
            cells["B2"].PutValue(123);
            cells["C3"].PutValue(DateTime.Now);

            // Obtener la altura estándar en píxeles
            int standardHeight = cells.StandardHeightPixels;
            Console.WriteLine("Standard row height in pixels: " + standardHeight);

            // Mostrar alturas de fila (debe coincidir con la altura estándar)
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches standard: {rowHeight == standardHeight}");
            }

            // Cambiar la altura estándar y verificar
            cells.StandardHeight = 20; // Set in points
            int newStandardHeight = cells.StandardHeightPixels;
            Console.WriteLine("\nNew standard height in pixels: " + newStandardHeight);

            // Verificar que todas las filas ahora tengan la nueva altura
            for (int i = 0; i < 5; i++)
            {
                int rowHeight = cells.GetRowHeightPixel(i);
                Console.WriteLine($"Row {i} height: {rowHeight}px");
                Console.WriteLine($"Matches new standard: {rowHeight == newStandardHeight}");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


