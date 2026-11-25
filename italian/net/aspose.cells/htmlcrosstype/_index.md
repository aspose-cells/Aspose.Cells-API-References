---
title: "Enum HtmlCrossType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.HtmlCrossType enum. Rappresenta cinque tipi di stringa html cross"
type: docs
url: /it/net/aspose.cells/htmlcrosstype/
---
## HtmlCrossType enumeration

Rappresenta cinque tipi di stringa incrociata HTML.

```csharp
public enum HtmlCrossType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Visualizza come MS Excel, dipende dalla cella successiva. Se la cella successiva è nulla, la stringa verrà incrociata, altrimenti verrà troncata |
| MSExport | `1` | Visualizza la stringa come MS Excel esportando html. |
| Cross | `2` | Visualizza la stringa HTML cross, questa prestazione per la creazione di grandi file html sarà più di dieci volte più veloce rispetto all'impostazione del valore su Default o FitToCell. |
| CrossHideRight | `3` | Visualizza la stringa HTML cross e nascondi la stringa a destra quando i testi si sovrappongono. |
| FitToCell | `4` | Visualizza solo la stringa entro la larghezza della cella. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHtmlCrossTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);
            
            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Imposta il tipo cross su MSExport
            options.HtmlCrossStringType = HtmlCrossType.MSExport;
            
            // Salva la cartella di lavoro con le opzioni HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with HtmlCrossType.MSExport");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


