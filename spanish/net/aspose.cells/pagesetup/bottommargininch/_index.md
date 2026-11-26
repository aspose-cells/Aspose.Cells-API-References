---
title: "PageSetup.BottomMarginInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el tamaño del margen inferior en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells/pagesetup/bottommargininch/
---
## PageSetup.BottomMarginInch property

Representa el tamaño del margen inferior, en unidades de pulgadas.

```csharp
public double BottomMarginInch { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginInchDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder al PageSetup de la primera hoja de cálculo
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Establecer varios márgenes en pulgadas
            setup.HeaderMarginInch = 0.1;
            setup.FooterMarginInch = 0.2;
            setup.TopMarginInch = 0.3;
            setup.BottomMarginInch = 0.4; // Demonstrating BottomMarginInch property
            setup.LeftMarginInch = 0.5;
            setup.RightMarginInch = 0.6;
            
            // Guarda el libro de trabajo
            workbook.Save("PageMarginsDemo.xlsx");
            
            // Mostrar confirmación
            Console.WriteLine("Workbook saved with bottom margin set to: " + setup.BottomMarginInch + " inches");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


