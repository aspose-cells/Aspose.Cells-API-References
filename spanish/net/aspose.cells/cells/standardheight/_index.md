---
title: "Cells.StandardHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo en unidades de puntos"
type: docs
url: /es/net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de puntos.

```csharp
public double StandardHeight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenga y muestre la altura estándar
            double standardHeight = worksheet.Cells.StandardHeight;
            Console.WriteLine("Standard Height: " + standardHeight);
            
            // Establezca una nueva altura estándar
            worksheet.Cells.StandardHeight = 20;
            Console.WriteLine("New Standard Height: " + worksheet.Cells.StandardHeight);
            
            // Guarda el libro de trabajo
            workbook.Save("StandardHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


