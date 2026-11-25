---
title: "Classe CellImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.CellImage. Rappresenta un collegamento ipertestuale con src immagine"
type: docs
url: /it/net/aspose.cells.gridweb.data/cellimage/
---
## CellImage class

Rappresenta un collegamento ipertestuale con sorgente immagine.

```csharp
public class CellImage : Hyperlink
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | Ottiene o imposta il tipo di azione del collegamento ipertestuale. Può essere ActionTpye.UrlLink o ActionType.CellCommand. Il tipo UrlLink indica che il collegamento è un link a una pagina web o a una mail. Per esempio: "http://www.aspose.com" o "mailto:admin@aspose.com". Il tipo CellCommand indica che il collegamento attiverà un evento CellCommand, e puoi gestire questo evento.(Ereditato da [`Hyperlink`](../hyperlink/).) |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | Ottiene l'intervallo del collegamento ipertestuale.(Ereditato da [`Hyperlink`](../hyperlink/).) |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | Ottiene o imposta il nome del Cell Command.(Ereditato da [`Hyperlink`](../hyperlink/).) |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | Indica se scartare l'input dell'utente nel browser client quando l'utente fa clic su questo collegamento CellCommand. Può essere usato come azione di "annullamento".(Ereditato da [`Hyperlink`](../hyperlink/).) |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | Ottiene o imposta l'URL dell'immagine del collegamento ipertestuale. Se impostato a null o a stringa vuota, il collegamento mostrerà solo il suo testo.(Ereditato da [`Hyperlink`](../hyperlink/).) |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } | (Ereditato da [`Hyperlink`](../hyperlink/).) |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | Ottiene o imposta il testo visualizzato del collegamento ipertestuale.(Ereditato da [`Hyperlink`](../hyperlink/).) |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | Ottiene o imposta il tooltip del collegamento ipertestuale.(Ereditato da [`Hyperlink`](../hyperlink/).) |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | Ottiene o imposta la stringa URL.(Ereditato da [`Hyperlink`](../hyperlink/).) |

### Vedi anche

* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


