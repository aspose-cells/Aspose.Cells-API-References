---
title: "HorizontalPageBreak.Row"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HorizontalPageBreak. Restituisce l'indice della riga basato su zero"
type: docs
url: /it/net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Restituisce l'indice della riga basato su zero.

```csharp
public int Row { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi interruzioni di pagina orizzontali
            worksheet.HorizontalPageBreaks.Add(6);
            worksheet.HorizontalPageBreaks.Add(12);

            // Ottieni la collezione delle interruzioni di pagina orizzontali
            HorizontalPageBreakCollection breaks = worksheet.HorizontalPageBreaks;

            // Visualizza i numeri di riga delle interruzioni di pagina
            Console.WriteLine("Page break at row: " + breaks[0].Row);
            Console.WriteLine("Page break at row: " + breaks[1].Row);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


