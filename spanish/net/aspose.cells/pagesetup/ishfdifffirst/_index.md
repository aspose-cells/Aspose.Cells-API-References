---
title: "PageSetup.IsHFDiffFirst"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. True significa que el encabezado/pie de página de la primera página es diferente al de las demás páginas"
type: docs
url: /es/net/aspose.cells/pagesetup/ishfdifffirst/
---
## PageSetup.IsHFDiffFirst property

True significa que el encabezado/pie de página de la primera página es diferente al de las demás páginas.

```csharp
public bool IsHFDiffFirst { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsHFDiffFirstDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceder a PageSetup
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establecer encabezados/pies de página diferentes para la primera página
            pageSetup.IsHFDiffFirst = true;
            
            // Establecer encabezados/pies de página
            pageSetup.SetFirstPageHeader(0, "First Page Header");
            pageSetup.SetHeader(0, "Standard Header");
            
            // Guarda el libro de trabajo
            workbook.Save("PageSetup_IsHFDiffFirst_Example.xlsx");
            
            // Recargar el libro para verificar la configuración
            Workbook loadedWorkbook = new Workbook("PageSetup_IsHFDiffFirst_Example.xlsx");
            PageSetup loadedPageSetup = loadedWorkbook.Worksheets[0].PageSetup;
            
            // Mostrar verificación
            Console.WriteLine("IsHFDiffFirst: " + loadedPageSetup.IsHFDiffFirst);
            Console.WriteLine("First Page Header: " + loadedPageSetup.GetFirstPageHeader(0));
            Console.WriteLine("Standard Header: " + loadedPageSetup.GetHeader(0));
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


