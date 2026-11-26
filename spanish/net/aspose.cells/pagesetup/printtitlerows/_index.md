---
title: "PageSetup.PrintTitleRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa las filas que contienen las celdas que se repetirán en la parte superior de cada página"
type: docs
url: /es/net/aspose.cells/pagesetup/printtitlerows/
---
## PageSetup.PrintTitleRows property

Representa las filas que contienen las celdas que se repiten en la parte superior de cada página.

```csharp
public string PrintTitleRows { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintTitleRowsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Data " + (i-1));
            }
            
            // Acceder a la configuración de página
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Establecer filas de título de impresión (la primera fila se repetirá en cada página impresa)
            pageSetup.PrintTitleRows = "$1:$1";
            
            // Guarda el libro de trabajo
            workbook.Save("PrintTitleRowsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


