---
title: "Worksheet.ShowFormulas"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet property. Indica si se deben mostrar las fórmulas o sus resultados"
type: docs
url: /es/net/aspose.cells/worksheet/showformulas/
---
## Worksheet.ShowFormulas property

Indica si se deben mostrar las fórmulas o sus resultados.

```csharp
public bool ShowFormulas { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShowFormulasDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer fórmula en la celda A1
            worksheet.Cells["A1"].Formula = "=1+2+3";
            
            // Mostrar inicialmente el valor calculado
            worksheet.ShowFormulas = false;
            Console.WriteLine("ShowFormulas OFF: " + worksheet.Cells["A1"].StringValue);

            // Alternar para mostrar el texto de la fórmula
            worksheet.ShowFormulas = true;
            Console.WriteLine("ShowFormulas ON: " + worksheet.Cells["A1"].StringValue);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


