---
title: "PageSetup.FirstPageNumber"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa el número de la primera página que se usará cuando se imprima esta hoja"
type: docs
url: /es/net/aspose.cells/pagesetup/firstpagenumber/
---
## PageSetup.FirstPageNumber property

Representa el número de la primera página que se usará cuando se imprima esta hoja.

```csharp
public int FirstPageNumber { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFirstPageNumberDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer propiedades de configuración de página
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            
            // Imprime los resultados
            Console.WriteLine("IsAutoFirstPageNumber: " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("FirstPageNumber: " + worksheet.PageSetup.FirstPageNumber);
            
            // Guarda el libro de trabajo
            workbook.Save("PageSetupFirstPageNumberDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


