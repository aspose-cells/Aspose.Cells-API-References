---
title: "PageSetup.HeaderMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa la distancia desde la parte superior de la página hasta el encabezado en unidades de centímetros"
type: docs
url: /es/net/aspose.cells/pagesetup/headermargin/
---
## PageSetup.HeaderMargin property

Representa la distancia desde la parte superior de la página hasta el encabezado, en unidades de centímetros.

```csharp
public double HeaderMargin { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer el margen del encabezado en centímetros
            pageSetup.HeaderMargin = 1.5;

            // Verificar que el margen del encabezado se haya establecido
            Console.WriteLine("Header Margin: " + pageSetup.HeaderMargin + " cm");

            // Guarda el libro de trabajo
            workbook.Save("HeaderMarginDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


