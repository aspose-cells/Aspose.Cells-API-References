---
title: "PageSetup.IsHFScaleWithDoc"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Indica si el encabezado y pie de página se escalan con el escalado del documento. Solo se aplica a Excel 2007."
type: docs
url: /es/net/aspose.cells/pagesetup/ishfscalewithdoc/
---
## PageSetup.IsHFScaleWithDoc property

Indica si el encabezado y pie de página se escalan con el escalado del documento. Solo se aplica a Excel 2007.

```csharp
public bool IsHFScaleWithDoc { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFScaleWithDocDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer configuración básica de página
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;

            // Demostrar la propiedad IsHFScaleWithDoc
            pageSetup.IsHFScaleWithDoc = true;
            Console.WriteLine("Header/Footer scaling with document is set to: " + pageSetup.IsHFScaleWithDoc);

            // Guarda el libro de trabajo
            workbook.Save("PageSetup_IsHFScaleWithDoc_Demo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


