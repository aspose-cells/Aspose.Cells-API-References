---
title: "VerticalPageBreak.EndRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà VerticalPageBreak. Ottiene l'indice di riga finale del salto di pagina verticale"
type: docs
url: /it/net/aspose.cells/verticalpagebreak/endrow/
---
## VerticalPageBreak.EndRow property

Restituisce l'indice della riga finale dell'interruzione di pagina verticale.

```csharp
public int EndRow { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyEndRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un salto di pagina verticale che copre le righe da 3 a 8 nella colonna C (indice 2)
            worksheet.VerticalPageBreaks.Add("C3:C8");

            // Ottieni il primo salto di pagina verticale
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            
            // Visualizza la riga finale del salto di pagina
            Console.WriteLine("Vertical Page Break End Row: " + vpb.EndRow);
            
            // Poiché EndRow è di sola lettura, dimostreremo come ottenerlo ma non impostarlo
            // La riga seguente è rimossa poiché causa un errore di compilazione:
            // vpb.EndRow = 10;
            
            // Invece, aggiungeremo un altro salto di pagina con una riga finale diversa
            worksheet.VerticalPageBreaks.Add("C3:C10");
            VerticalPageBreak vpb2 = worksheet.VerticalPageBreaks[1];
            Console.WriteLine("Second Page Break End Row: " + vpb2.EndRow);
        }
    }
}
```

### Vedi anche

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


