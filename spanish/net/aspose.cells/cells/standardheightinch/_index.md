---
title: "Cells.StandardHeightInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/cells/standardheightinch/
---
## Cells.StandardHeightInch property

Obtiene o establece la altura de fila predeterminada en esta hoja de cálculo, en unidades de pulgadas.

```csharp
public double StandardHeightInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtener la altura estándar en pulgadas
            double standardHeightInch = worksheet.Cells.StandardHeightInch;
            Console.WriteLine("Standard Height in Inches: " + standardHeightInch);
            
            // Establecer una nueva altura estándar (1 pulgada)
            worksheet.Cells.StandardHeightInch = 1.0;
            Console.WriteLine("New Standard Height in Inches: " + worksheet.Cells.StandardHeightInch);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


