---
title: "VerticalPageBreak.Column"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VerticalPageBreak. Ottiene l'indice di colonna del salto di pagina verticale"
type: docs
url: /it/net/aspose.cells/verticalpagebreak/column/
---
## VerticalPageBreak.Column property

Restituisce l'indice della colonna dell'interruzione di pagina verticale.

```csharp
public int Column { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi salti di pagina verticali nelle colonne 4 e 8
            worksheet.VerticalPageBreaks.Add(4);
            worksheet.VerticalPageBreaks.Add(8);

            // Ottieni la raccolta delle interruzioni di pagina verticali
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;

            // Visualizza le informazioni su ogni salto di pagina verticale
            Console.WriteLine("Vertical Page Breaks Count: " + vpagebreaks.Count);
            
            foreach (VerticalPageBreak vpagebreak in vpagebreaks)
            {
                Console.WriteLine("\nPage Break at Column: " + vpagebreak.Column);
                Console.WriteLine("Start Row: " + vpagebreak.StartRow);
                Console.WriteLine("End Row: " + vpagebreak.EndRow);
            }

            // Salva la cartella di lavoro
            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


