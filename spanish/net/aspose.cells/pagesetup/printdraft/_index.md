---
title: "PageSetup.PrintDraft"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa si la hoja se imprimirá sin gráficos"
type: docs
url: /es/net/aspose.cells/pagesetup/printdraft/
---
## PageSetup.PrintDraft property

Representa si la hoja se imprimirá sin gráficos.

```csharp
public bool PrintDraft { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintDraftDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder al objeto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer la propiedad PrintDraft a true
            pageSetup.PrintDraft = true;
            Console.WriteLine("PrintDraft set to: " + pageSetup.PrintDraft);

            // Cambiar la propiedad PrintDraft a false
            pageSetup.PrintDraft = false;
            Console.WriteLine("PrintDraft changed to: " + pageSetup.PrintDraft);

            // Guarda el libro de trabajo
            workbook.Save("PageSetup_PrintDraft_Example.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


