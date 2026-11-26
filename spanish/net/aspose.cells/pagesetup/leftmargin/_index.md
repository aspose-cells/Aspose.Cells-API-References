---
title: "PageSetup.LeftMargin"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el tamaño del margen izquierdo en unidades de centímetros"
type: docs
url: /es/net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

Representa el tamaño del margen izquierdo, en unidades de centímetros.

```csharp
public double LeftMargin { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer algunos datos de muestra
            sheet.Cells["A1"].PutValue("Left Margin Demonstration");
            sheet.Cells["A2"].PutValue("This shows how to set page margins");

            // Establecer margen izquierdo (en pulgadas)
            sheet.PageSetup.LeftMargin = 1.5;

            // Imprime el valor del margen izquierdo en la consola
            Console.WriteLine("Left Margin set to: " + sheet.PageSetup.LeftMargin + " inches");

            // Guarda en PDF para demostrar el margen
            string outputPath = "LeftMarginDemo.pdf";
            workbook.Save(outputPath, SaveFormat.Pdf);

            Console.WriteLine("File saved with left margin: " + outputPath);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


