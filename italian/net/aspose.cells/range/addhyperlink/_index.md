---
title: "Range.AddHyperlink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Range. Aggiunge un collegamento ipertestuale a una cella specificata o a un intervallo di celle"
type: docs
url: /it/net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

Aggiunge un hyperlink a una cella specificata o a un intervallo di celle.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| address | String | Indirizzo del collegamento ipertestuale. |
| textToDisplay | String | Il testo da visualizzare per il collegamento ipertestuale specificato. |
| screenTip | String | Il testo screenTip per il collegamento ipertestuale specificato. |

### Valore di ritorno

[`Hyperlink`](../../hyperlink/) object.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAddHyperlinkWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
            
            // Aggiungi un collegamento ipertestuale con indirizzo, testo da visualizzare e suggerimento
            range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
            
            // Salva la cartella di lavoro
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


