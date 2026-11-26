---
title: "PageSetup.ClearHeaderFooter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PageSetup. Borra la configuración de encabezado y pie de página"
type: docs
url: /es/net/aspose.cells/pagesetup/clearheaderfooter/
---
## PageSetup.ClearHeaderFooter method

Borra la configuración del encabezado y pie de página.

```csharp
public void ClearHeaderFooter()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodClearHeaderFooterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer encabezados y pies de página iniciales
            pageSetup.SetHeader(0, "Initial Left Header");
            pageSetup.SetFooter(0, "Initial Left Footer");

            Console.WriteLine("Before ClearHeaderFooter:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));

            // Borrar encabezados y pies de página
            pageSetup.ClearHeaderFooter();

            Console.WriteLine("\nAfter ClearHeaderFooter:");
            Console.WriteLine("Header: " + (string.IsNullOrEmpty(pageSetup.GetHeader(0)) ? "Cleared" : "Not Cleared"));
            Console.WriteLine("Footer: " + (string.IsNullOrEmpty(pageSetup.GetFooter(0)) ? "Cleared" : "Not Cleared"));

            // Establecer nuevos encabezados y pies de página después de borrar
            pageSetup.SetHeader(0, "New Left Header");
            pageSetup.SetFooter(0, "New Left Footer");

            Console.WriteLine("\nAfter Setting New Values:");
            Console.WriteLine("Header: " + pageSetup.GetHeader(0));
            Console.WriteLine("Footer: " + pageSetup.GetFooter(0));
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


