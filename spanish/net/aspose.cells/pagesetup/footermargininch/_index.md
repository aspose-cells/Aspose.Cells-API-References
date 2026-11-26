---
title: "PageSetup.FooterMarginInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa la distancia desde la parte inferior de la página hasta el pie de página en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/pagesetup/footermargininch/
---
## PageSetup.FooterMarginInch property

Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de pulgadas.

```csharp
public double FooterMarginInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginInchDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo y su PageSetup
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establecer el margen del pie de página en pulgadas
            pageSetup.FooterMarginInch = 0.5;
            
            // Establecer otros márgenes para demostración
            pageSetup.HeaderMarginInch = 0.3;
            pageSetup.TopMarginInch = 1.0;
            pageSetup.BottomMarginInch = 1.0;
            pageSetup.LeftMarginInch = 0.75;
            pageSetup.RightMarginInch = 0.75;
            
            // Guarda el libro de trabajo
            workbook.Save("PageSetupMargins.xlsx");
            
            // Imprimir confirmación
            Console.WriteLine("Footer margin set to: " + pageSetup.FooterMarginInch + " inches");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


