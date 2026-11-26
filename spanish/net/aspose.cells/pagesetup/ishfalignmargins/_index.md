---
title: "PageSetup.IsHFAlignMargins"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Indica si los márgenes de encabezado y pie de página están alineados con los márgenes de la página. Si esta propiedad es verdadera, el encabezado y pie de página izquierdo se alinearán con el margen izquierdo y el encabezado y pie de página derecho se alinearán con el margen derecho. Esta opción está habilitada por defecto"
type: docs
url: /es/net/aspose.cells/pagesetup/ishfalignmargins/
---
## PageSetup.IsHFAlignMargins property

Indica si los márgenes del encabezado y pie de página están alineados con los márgenes de la página. Si esta propiedad es verdadera, el encabezado y pie de página izquierdo se alinearán con el margen izquierdo, y el encabezado y pie de página derecho se alinearán con el margen derecho. Esta opción está habilitada por defecto.

```csharp
public bool IsHFAlignMargins { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFAlignMarginsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer IsHFAlignMargins a verdadero
            pageSetup.IsHFAlignMargins = true;
            Console.WriteLine("IsHFAlignMargins set to: " + pageSetup.IsHFAlignMargins);

            // Cambiar IsHFAlignMargins a falso
            pageSetup.IsHFAlignMargins = false;
            Console.WriteLine("IsHFAlignMargins changed to: " + pageSetup.IsHFAlignMargins);

            // Guarda el libro de trabajo
            workbook.Save("PageSetup_IsHFAlignMargins_Example.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


