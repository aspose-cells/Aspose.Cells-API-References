---
title: "PageSetup.PrintGridlines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Indica si las líneas de cuadrícula de las celdas se imprimen en la página"
type: docs
url: /es/net/aspose.cells/pagesetup/printgridlines/
---
## PageSetup.PrintGridlines property

Representa si las líneas de cuadrícula de las celdas se imprimen en la página.

```csharp
public bool PrintGridlines { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintGridlinesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Colocar datos de ejemplo en la celda
            worksheet.Cells["A1"].PutValue("PrintGridlines Property Demo");
            worksheet.Cells["A3"].PutValue("Gridlines will ");
            worksheet.Cells["B3"].PutValue(worksheet.PageSetup.PrintGridlines ? "appear" : "not appear");
            worksheet.Cells["A4"].PutValue("when printing this sheet.");

            // Alternar la propiedad PrintGridlines
            worksheet.PageSetup.PrintGridlines = true;
            
            // Guarda el libro de trabajo
            workbook.Save("PrintGridlinesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


