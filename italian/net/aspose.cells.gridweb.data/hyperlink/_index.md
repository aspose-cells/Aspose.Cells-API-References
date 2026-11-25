---
title: "Classe Hyperlink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.Hyperlink."
type: docs
url: /it/net/aspose.cells.gridweb.data/hyperlink/
---
## Hyperlink class

```csharp
[Obsolete("This class is obsolete; use GridHyperlink instead")]
public class Hyperlink
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Ottiene o imposta il tipo di azione dell'ipertesto. Può essere ActionTpye.UrlLink o ActionType.CellCommand. Il tipo UrlLink indica che l'ipertesto è un collegamento a una pagina web o a una mail. Per esempio: "http://www.aspose.com" o "mailto:admin@aspose.com". Il tipo CellCommand indica che l'ipertesto genererà un evento CellCommand, e potrai gestire questo evento. |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Ottiene l'intervallo dell'hyperlink. |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Ottiene o imposta il nome del Cell Command. |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Indica se scartare l'input dell'utente nel browser client quando l'utente clicca su questo collegamento ipertestuale CellCommand. Può essere usato come azione di \"undo\". |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Ottiene o imposta l'URL dell'immagine dell'ipertesto. Se impostato a null o a stringa vuota, l'ipertesto mostrerà solo il suo testo. |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } |  |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Ottiene o imposta il testo visualizzato dell'ipertesto. |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Ottiene o imposta il tooltip dell'ipertesto. |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Ottiene o imposta la stringa URL. |

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


