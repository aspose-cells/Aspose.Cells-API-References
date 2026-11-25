---
title: "HighlightChangesOptions.HighlightChangesOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore HighlightChangesOptions. Rappresenta le opzioni di evidenziazione delle revisioni o delle modifiche di file Excel condivisi"
type: docs
url: /it/net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

Rappresenta le opzioni per evidenziare le revisioni o le modifiche dei file Excel condivisi.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| highlightOnScreen | Booleano | Indica se le modifiche sono evidenziate sullo schermo. |
| listOnNewSheet | Booleano | Indica se elencare le modifiche in un nuovo foglio di lavoro. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Crea HighlightChangesOptions con parametri booleani
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            
            // Simula il tracciamento delle modifiche (normalmente avresti revisioni reali)
            Console.WriteLine("HighlightChangesOptions created with:");
            Console.WriteLine($"First parameter (show changes): {true}");
            Console.WriteLine($"Second parameter (changes on new sheet): {true}");
            
            // Salva la cartella di lavoro
            workbook.Save("HighlightChangesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


