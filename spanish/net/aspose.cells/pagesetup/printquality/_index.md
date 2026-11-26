---
title: "PageSetup.PrintQuality"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa la calidad de impresión"
type: docs
url: /es/net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

Representa la calidad de impresión.

```csharp
public int PrintQuality { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintQualityDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer la calidad de impresión a 144 ppp
            worksheet.PageSetup.PrintQuality = 144;
            
            // Imprimir la configuración actual de calidad de impresión
            Console.WriteLine("Print Quality: " + worksheet.PageSetup.PrintQuality);
            
            // Guarda el libro de trabajo
            workbook.Save("PrintQualityDemo.xls");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


