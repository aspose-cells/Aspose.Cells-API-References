---
title: "PageSetup.PrintErrors"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Especifica el tipo de error de impresión mostrado"
type: docs
url: /es/net/aspose.cells/pagesetup/printerrors/
---
## PageSetup.PrintErrors property

Especifica el tipo de error de impresión mostrado.

```csharp
public PrintErrorsType PrintErrors { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintErrorsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Establecer errores de impresión para que se muestren en blanco
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            Console.WriteLine("PrintErrors set to: " + sheet.PageSetup.PrintErrors);
            
            // Cambiar errores de impresión para que se muestren como guiones
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            Console.WriteLine("PrintErrors changed to: " + sheet.PageSetup.PrintErrors);
            
            // Guarda el libro de trabajo
            workbook.Save("PrintErrorsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


