---
title: "VerticalPageBreak.StartRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VerticalPageBreak. Ottiene l'indice di riga iniziale del salto di pagina verticale"
type: docs
url: /it/net/aspose.cells/verticalpagebreak/startrow/
---
## VerticalPageBreak.StartRow property

Restituisce l'indice della riga iniziale dell'interruzione di pagina verticale.

```csharp
public int StartRow { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyStartRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi salti di pagina verticali con la riga iniziale desiderata (2) inizialmente
            worksheet.VerticalPageBreaks.Add(2, 0, 10);
            VerticalPageBreak vPageBreak = worksheet.VerticalPageBreaks[0];

            // Visualizza la proprietà StartRow
            Console.WriteLine("Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Poiché StartRow è di sola lettura, dobbiamo rimuovere e riaggiungere per modificarla
            worksheet.VerticalPageBreaks.RemoveAt(0);
            worksheet.VerticalPageBreaks.Add(5, 0, 10);
            vPageBreak = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Modified Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Salva la cartella di lavoro
            workbook.Save("VerticalPageBreakExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


