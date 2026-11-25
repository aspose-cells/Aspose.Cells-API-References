---
title: "Enum TextStrikeType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.TextStrikeType. Questo tipo specifica il tipo di barratura"
type: docs
url: /it/net/aspose.cells/textstriketype/
---
## TextStrikeType enumeration

Questo tipo specifica il tipo di barrato.

```csharp
public enum TextStrikeType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Single | `0` | Una singola barratura applicata al testo. |
| Double | `1` | Una doppia barratura applicata al testo. Funziona solo per il testo di forme o grafici. |
| None | `2` | Nessuna barratura è applicata al testo. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextStrikeTypeDemo
    {
        public static void TextStrikeTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            // Ottieni il riferimento del primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            // Accedere alla cella "A1" dal foglio di lavoro
            Cell cell = worksheet.Cells["A1"];
            // Aggiungere un valore alla cella "A1"
            cell.PutValue("Hello Aspose!");

            // Accesso al font della cella
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Impostazione del tipo di barratura su Single
            font.StrikeType = TextStrikeType.Single;

            // Applica lo stile alla cella
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("TextStrikeTypeExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


