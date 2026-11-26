---
title: "PageSetup.TopMarginInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el tamaño del margen superior en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/pagesetup/topmargininch/
---
## PageSetup.TopMarginInch property

Representa el tamaño del margen superior, en unidades de pulgadas.

```csharp
public double TopMarginInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginInchDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer el margen superior a 1.5 pulgadas
            sheet.PageSetup.TopMarginInch = 1.5;

            // Obtener e imprimir el valor del margen superior
            Console.WriteLine("Top Margin (inches): " + sheet.PageSetup.TopMarginInch);

            // Guarda el libro de trabajo
            workbook.Save("PageSetup_TopMarginInch_Example.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


