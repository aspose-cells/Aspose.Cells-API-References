---
title: "Cells.StandardWidthInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells. Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/cells/standardwidthinch/
---
## Cells.StandardWidthInch property

Obtiene o establece el ancho de columna predeterminado en la hoja de cálculo, en unidades de pulgadas.

```csharp
public double StandardWidthInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStandardWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer el ancho de columna estándar en pulgadas
            worksheet.Cells.StandardWidthInch = 1.5;

            // Establecer el ancho de columna específico en pulgadas para demostración
            worksheet.Cells.SetColumnWidthInch(1, 2.0);

            // Guarda el libro de trabajo
            workbook.Save("StandardWidthInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


