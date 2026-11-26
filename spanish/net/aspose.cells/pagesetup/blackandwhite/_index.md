---
title: "PageSetup.BlackAndWhite"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa si los elementos del documento se imprimirán en blanco y negro"
type: docs
url: /es/net/aspose.cells/pagesetup/blackandwhite/
---
## PageSetup.BlackAndWhite property

Representa si los elementos del documento se imprimirán en blanco y negro.

```csharp
public bool BlackAndWhite { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBlackAndWhiteDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener el objeto PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Establecer la propiedad BlackAndWhite a true
            pageSetup.BlackAndWhite = true;
            Console.WriteLine("BlackAndWhite set to: " + pageSetup.BlackAndWhite);

            // Cambiar la propiedad BlackAndWhite a false
            pageSetup.BlackAndWhite = false;
            Console.WriteLine("BlackAndWhite changed to: " + pageSetup.BlackAndWhite);

            // Guarda el libro de trabajo
            workbook.Save("PageSetupBlackAndWhiteDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


