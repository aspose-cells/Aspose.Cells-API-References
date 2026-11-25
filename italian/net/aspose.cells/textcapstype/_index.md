---
title: "Enum TextCapsType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.TextCapsType. Questo tipo specifica i tipi di maiuscole del testo"
type: docs
url: /it/net/aspose.cells/textcapstype/
---
## TextCapsType enumeration

Questo tipo specifica i tipi di maiuscole del testo.

```csharp
public enum TextCapsType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna maiuscola |
| All | `1` | Applica tutte le maiuscole al testo. |
| Small | `2` | Applica le maiuscole piccole al testo. |

### Osservazioni

Può essere applicato solo a grafico e forma.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TextCapsTypeDemo
    {
        public static void TextCapsTypeExample()
        {
            // Codice aggiuntivo per dimostrare come l'istanza potrebbe essere utilizzata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta il valore di una cella
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // Ottieni lo stile della cella
            Style style = cell.GetStyle();

            // Imposta il tipo di maiuscole del carattere su Tutte le maiuscole
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // Applica lo stile alla cella
            cell.SetStyle(style);

            // Salva la cartella di lavoro
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


