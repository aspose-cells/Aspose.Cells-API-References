---
title: "Classe ReplaceOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ReplaceOptions. Rappresenta le opzioni di sostituzione"
type: docs
url: /it/net/aspose.cells/replaceoptions/
---
## ReplaceOptions class

Rappresenta le opzioni di sostituzione.

```csharp
public class ReplaceOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ReplaceOptions](replaceoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CaseSensitive](../../aspose.cells/replaceoptions/casesensitive/) { get; set; } | Indica se la stringa cercata è sensibile al maiuscolo/minuscolo. |
| [FontSettings](../../aspose.cells/replaceoptions/fontsettings/) { get; set; } | Le impostazioni di formattazione ricca per il testo sostituito. |
| [MatchEntireCellContents](../../aspose.cells/replaceoptions/matchentirecellcontents/) { get; set; } | Indica se corrispondere all'intero contenuto delle celle |
| [RegexKey](../../aspose.cells/replaceoptions/regexkey/) { get; set; } | Indica se la chiave cercata è una regex. Se vero, la chiave cercata verrà interpretata come regex. |
| [StyleFlags](../../aspose.cells/replaceoptions/styleflags/) { get; set; } | Ottiene e imposta i flag per l'applicazione delle impostazioni del carattere. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReplaceOptionsDemo
    {
        public static void ReplaceOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // Crea ReplaceOptions
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // Sostituisci "Hello" con "Hi" nel foglio di lavoro
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // Restituisci il numero di sostituzioni effettuate
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // Salva la cartella di lavoro
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


