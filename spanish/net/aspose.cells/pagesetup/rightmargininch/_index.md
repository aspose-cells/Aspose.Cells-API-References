---
title: "PageSetup.RightMarginInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el tamaño del margen derecho en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/pagesetup/rightmargininch/
---
## PageSetup.RightMarginInch property

Representa el tamaño del margen derecho, en unidades de pulgadas.

```csharp
public double RightMarginInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyRightMarginInchDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a PageSetup y establecer RightMarginInch
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.RightMarginInch = 0.75; // Set right margin to 0.75 inches

            // Agrega algunos datos de ejemplo para ver el efecto
            worksheet.Cells["A1"].PutValue("Right Margin Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["B" + i].PutValue("Sample Data " + i);
            }

            // Guarda el libro de trabajo
            workbook.Save("RightMarginInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


