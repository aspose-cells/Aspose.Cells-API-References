---
title: "PageSetup.LeftMarginInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PageSetup property. Representa el tamaño del margen izquierdo en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/pagesetup/leftmargininch/
---
## PageSetup.LeftMarginInch property

Representa el tamaño del margen izquierdo, en unidades de pulgadas.

```csharp
public double LeftMarginInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginInchDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Establezca el margen izquierdo en pulgadas (0.39 pulgadas = ~1 cm)
            pageSetup.LeftMarginInch = 0.39;

            // Agregue algunos datos para demostrar el margen
            worksheet.Cells["A1"].PutValue("Left Margin Demonstration");
            worksheet.Cells["A2"].PutValue("Left margin set to 0.39 inches");

            // Guarda el libro de trabajo
            workbook.Save("LeftMarginInchDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


