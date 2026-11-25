---
title: "Cell.Replace"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Sostituisci il testo della cella con le opzioni"
type: docs
url: /it/net/aspose.cells/cell/replace/
---
## Cell.Replace method

Sostituisce il testo della cella con le opzioni.

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| segnaposto | String | Segnaposto cella |
| nuovoValore | String | Valore stringa da sostituire |
| opzioni | ReplaceOptions | Le opzioni di sostituzione |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("hello world");
            worksheet.Cells["A3"].PutValue("HELLO WORLD");
            worksheet.Cells["B1"].PutValue("Replaced");

            // Crea le opzioni di sostituzione
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            options.MatchEntireCellContents = false;

            // Ottieni le impostazioni del carattere dalla cella B1 da applicare alle sostituzioni
            options.FontSettings = worksheet.Cells["B1"].GetCharacters();

            // Sostituisci tutte le varianti di "hello" con "Hi" usando le opzioni
            foreach (Cell cell in worksheet.Cells)
            {
                cell.Replace("Hello", "Hi", options);
            }

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


