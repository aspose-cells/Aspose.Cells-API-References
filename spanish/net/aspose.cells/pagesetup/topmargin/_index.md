---
title: "PageSetup.TopMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el tamaño del margen superior en unidades de centímetros"
type: docs
url: /es/net/aspose.cells/pagesetup/topmargin/
---
## PageSetup.TopMargin property

Representa el tamaño del margen superior, en unidades de centímetros.

```csharp
public double TopMargin { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyTopMarginDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            sheet.Cells["A1"].PutValue("Top Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows the effect of TopMargin property");

            // Establecer propiedades de configuración de página
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.TopMargin = 2.0; // 2 inches top margin
            pageSetup.LeftMargin = 0.5;
            pageSetup.RightMargin = 0.5;
            pageSetup.BottomMargin = 1.0;

            // Guardar como PDF para demostrar los márgenes
            string outputPath = "TopMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("Document with top margin of 2 inches saved to: " + outputPath);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


