---
title: "HorizontalPageBreak.EndColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HorizontalPageBreak. Restituisce l'indice della colonna finale di questa interruzione di pagina orizzontale"
type: docs
url: /it/net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

Restituisce l'indice della colonna finale di questa interruzione di pagina orizzontale.

```csharp
public int EndColumn { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un'interruzione di pagina orizzontale alla riga 5, che si estende dalla colonna 2 alla 4
            int index = worksheet.HorizontalPageBreaks.Add(5, 2, 4);
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];

            // Visualizza la proprietà EndColumn
            Console.WriteLine("Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);

            // Poiché EndColumn è di sola lettura, è necessario rimuovere e riaggiungere l'interruzione di pagina per modificarla
            worksheet.HorizontalPageBreaks.RemoveAt(index);
            index = worksheet.HorizontalPageBreaks.Add(5, 2, 6);
            hPageBreak = worksheet.HorizontalPageBreaks[index];
            Console.WriteLine("Modified Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
        }
    }
}
```

### Vedi anche

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


