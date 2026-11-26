---
title: "PageSetup.BottomMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el tamaño del margen inferior en unidades de centímetros"
type: docs
url: /es/net/aspose.cells/pagesetup/bottommargin/
---
## PageSetup.BottomMargin property

Representa el tamaño del margen inferior, en unidades de centímetros.

```csharp
public double BottomMargin { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBottomMarginDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Sample Text for Margin Demonstration");
            
            // Configura la configuración de página con BottomMargin
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.BottomMargin = 0.5; // 0.5 inch bottom margin
            pageSetup.TopMargin = 1.0;    // 1 inch top margin
            pageSetup.LeftMargin = 0.75;  // 0.75 inch left margin
            pageSetup.RightMargin = 0.75; // 0.75 inch right margin

            // Guardar en PDF para demostrar los márgenes
            workbook.Save("PageMarginsDemo.pdf", SaveFormat.Pdf);

            Console.WriteLine("Document with bottom margin of 0.5 inches created successfully.");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


