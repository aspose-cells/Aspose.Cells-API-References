---
title: "PageSetup.FooterMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PageSetup property. Representa la distancia desde la parte inferior de la página hasta el pie de página en unidades de centímetros"
type: docs
url: /es/net/aspose.cells/pagesetup/footermargin/
---
## PageSetup.FooterMargin property

Representa la distancia desde la parte inferior de la página hasta el pie de página, en unidades de centímetros.

```csharp
public double FooterMargin { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Establezca el margen del pie de página en centímetros
            pageSetup.FooterMargin = 1.5;

            // Agregue contenido para ver el efecto
            worksheet.Cells["A1"].PutValue("Footer Margin Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates setting footer margin to 1.5 cm");

            // Establezca el texto del pie de página para que el margen sea visible
            pageSetup.SetFooter(0, "&A - Footer text to demonstrate margin");

            // Guarda el libro de trabajo
            workbook.Save("FooterMarginDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


