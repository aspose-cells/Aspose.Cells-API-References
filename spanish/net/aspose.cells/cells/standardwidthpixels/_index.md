---
title: "Cells.StandardWidthPixels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo en unidades de píxeles"
type: docs
url: /es/net/aspose.cells/cells/standardwidthpixels/
---
## Cells.StandardWidthPixels property

Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de píxeles.

```csharp
public int StandardWidthPixels { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthPixelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer y obtener el ancho estándar en píxeles
            cells.StandardWidthPixels = 104;
            Console.WriteLine("Standard Width in Pixels: " + cells.StandardWidthPixels);

            // Establecer y obtener el ancho estándar en caracteres
            cells.StandardWidth = 12.375;
            Console.WriteLine("Standard Width in Characters: " + cells.StandardWidth);

            // Establecer y obtener la altura estándar en puntos
            cells.StandardHeight = 14.25;
            Console.WriteLine("Standard Height in Points: " + cells.StandardHeight);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


