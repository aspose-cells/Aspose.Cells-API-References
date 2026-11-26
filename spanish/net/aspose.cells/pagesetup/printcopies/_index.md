---
title: "PageSetup.PrintCopies"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Obtiene y establece el número de copias a imprimir"
type: docs
url: /es/net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

Obtiene y establece el número de copias a imprimir.

```csharp
public int PrintCopies { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCopiesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer el número de copias de impresión a 3
            worksheet.PageSetup.PrintCopies = 3;
            
            // Mostrar la configuración actual de copias de impresión
            Console.WriteLine("Print Copies: " + worksheet.PageSetup.PrintCopies);
            
            // Guarda el libro de trabajo
            workbook.Save("PageSetup_PrintCopies_Output.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


