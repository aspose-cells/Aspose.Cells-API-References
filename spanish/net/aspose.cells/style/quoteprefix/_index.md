---
title: "Style.QuotePrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Indica si el valor de la celda comienza con una comilla simple"
type: docs
url: /es/net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Indica si el valor de la celda comienza con una comilla simple.

```csharp
public bool QuotePrefix { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceda a la celda B10 y establezca su valor
            Cell cell = worksheet.Cells["B10"];
            cell.PutValue("'12345"); // Note the single quote prefix

            // Obtén el estilo de la celda y habilita QuotePrefix
            Style style = cell.GetStyle();
            style.QuotePrefix = true;
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Verifica la propiedad QuotePrefix
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cell loadedCell = loadedWorkbook.Worksheets[0].Cells["B10"];
            Console.WriteLine("QuotePrefix is set: " + loadedCell.GetStyle().QuotePrefix);
        }
    }
}
```

### Ver también

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


