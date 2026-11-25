---
title: "Classe Hyperlink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Hyperlink. Incapsula l'oggetto che rappresenta un hyperlink"
type: docs
url: /it/net/aspose.cells/hyperlink/
---
## Hyperlink class

Incapsula l'oggetto che rappresenta un collegamento ipertestuale.

```csharp
public class Hyperlink
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Address](../../aspose.cells/hyperlink/address/) { get; set; } | Rappresenta l'indirizzo di un hyperlink. |
| [Area](../../aspose.cells/hyperlink/area/) { get; } | Ottiene l'intervallo dell'hyperlink. |
| [LinkType](../../aspose.cells/hyperlink/linktype/) { get; } | Ottiene il tipo di collegamento. |
| [ScreenTip](../../aspose.cells/hyperlink/screentip/) { get; set; } | Restituisce o imposta il testo ScreenTip per il collegamento ipertestuale specificato. |
| [TextToDisplay](../../aspose.cells/hyperlink/texttodisplay/) { get; set; } | Rappresenta il testo da visualizzare per il collegamento ipertestuale specificato. Il valore predefinito è l'indirizzo del collegamento ipertestuale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Delete](../../aspose.cells/hyperlink/delete/)() | Elimina questo collegamento ipertestuale |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkDemo
    {
        public static void HyperlinkExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            
            // Aggiungere un nuovo foglio di lavoro all'oggetto Workbook
            workbook.Worksheets.Add();
            
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiunta di un collegamento ipertestuale a un URL nella cella "A1"
            int index = worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");
            
            // Recupero di un collegamento ipertestuale per indice
            Hyperlink hyperlink = worksheet.Hyperlinks[index];
            
            // Impostazione del testo visualizzato di questo collegamento ipertestuale
            hyperlink.TextToDisplay = "Aspose";
            
            // Impostazione del testo ScreenTip per il collegamento ipertestuale
            hyperlink.ScreenTip = "Visit Aspose Website";
            
            // Salvataggio del file Excel
            workbook.Save("HyperlinkExample.xlsx");
            workbook.Save("HyperlinkExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


