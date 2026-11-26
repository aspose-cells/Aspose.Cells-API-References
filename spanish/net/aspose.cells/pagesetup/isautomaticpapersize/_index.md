---
title: "PageSetup.IsAutomaticPaperSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Indica si el tamaño del papel es automático"
type: docs
url: /es/net/aspose.cells/pagesetup/isautomaticpapersize/
---
## PageSetup.IsAutomaticPaperSize property

Indica si el tamaño del papel es automático.

```csharp
public bool IsAutomaticPaperSize { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutomaticPaperSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a la configuración de página
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Obtener el valor del tamaño de papel automático
            Console.WriteLine("Automatic Paper Size: " + pageSetup.IsAutomaticPaperSize);
            
            // Cree otro libro de trabajo con configuraciones diferentes
            Workbook workbook2 = new Workbook("example.xlsx");
            PageSetup pageSetup2 = workbook2.Worksheets[0].PageSetup;
            Console.WriteLine("Automatic Paper Size from file: " + pageSetup2.IsAutomaticPaperSize);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


