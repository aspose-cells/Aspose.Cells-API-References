---
title: "PageSetup.IsPercentScale"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Si esta propiedad es False, las propiedades FitToPagesWide y FitToPagesTall controlan cómo se escala la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/pagesetup/ispercentscale/
---
## PageSetup.IsPercentScale property

Si esta propiedad es False, las propiedades FitToPagesWide y FitToPagesTall controlan cómo se escala la hoja de cálculo.

```csharp
public bool IsPercentScale { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsPercentScaleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a PageSetup y establecer la escala al 80% (escala en porcentaje)
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.Zoom = 80;
            pageSetup.IsPercentScale = true;

            // Mostrar la configuración para demostrar IsPercentScale
            Console.WriteLine("Zoom: " + pageSetup.Zoom);
            Console.WriteLine("IsPercentScale: " + pageSetup.IsPercentScale);

            // Guarda el libro de trabajo
            workbook.Save("PageSetup_IsPercentScale_Output.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


