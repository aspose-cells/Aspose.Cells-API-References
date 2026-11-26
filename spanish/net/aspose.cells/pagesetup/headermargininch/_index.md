---
title: "PageSetup.HeaderMarginInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa la distancia desde la parte superior de la página hasta el encabezado en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/pagesetup/headermargininch/
---
## PageSetup.HeaderMarginInch property

Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de pulgadas.

```csharp
public double HeaderMarginInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginInchDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo y su PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer el margen del encabezado en pulgadas
            pageSetup.HeaderMarginInch = 0.5;
            
            // Establecer otros márgenes para demostración
            pageSetup.FooterMarginInch = 0.25;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;

            // Guarda el libro de trabajo
            workbook.Save("PageSetupMargins.xlsx");

            // Mostrar el valor del margen del encabezado
            Console.WriteLine("Header Margin (inches): " + pageSetup.HeaderMarginInch);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


