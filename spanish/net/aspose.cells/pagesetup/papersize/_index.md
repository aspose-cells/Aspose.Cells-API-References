---
title: "PageSetup.PaperSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el tamaño del papel"
type: docs
url: /es/net/aspose.cells/pagesetup/papersize/
---
## PageSetup.PaperSize property

Representa el tamaño del papel.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer el tamaño del papel a Sobre B6
            sheet.PageSetup.PaperSize = PaperSizeType.PaperEnvelopeB6;

            // Imprimir el tamaño de papel actual
            Console.WriteLine("Current paper size: " + sheet.PageSetup.PaperSize);

            // Guarda el libro de trabajo
            workbook.Save("PageSetup_PaperSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


