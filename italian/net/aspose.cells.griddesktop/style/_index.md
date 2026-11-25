---
title: "Classe Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridDesktop.Style classe. Rappresenta lo stile di visualizzazione dei documenti Excel, come colore del carattere, allineamento, bordo, ecc."
type: docs
url: /it/net/aspose.cells.griddesktop/style/
---
## Style class

Rappresenta lo stile di visualizzazione di un documento Excel, come font, colore, allineamento, bordo, ecc.

```csharp
public class Style
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Style](style/)(GridDesktop) | crea un nuovo Style per il controllo |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor/) { get; set; } | Ottiene o imposta il colore di sfondo della cella; se il modello di stile non è impostato su solido, avrà effetto. |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked/) { get; set; } | Ottiene o imposta un valore che indica se una cella può essere modificata o meno. |
| [Color](../../aspose.cells.griddesktop/style/color/) { get; set; } | Ottiene o imposta il colore di ombreggiatura della cella. Quando il modello è none, restituisce Color.Empty; quando il modello è BackgroundType.Solid, restituisce ForegroundColor; negli altri casi restituisce BackgroundColor. |
| [Custom](../../aspose.cells.griddesktop/style/custom/) { get; set; } | Rappresenta la stringa di formato numerico personalizzato di questo oggetto stile. Se il formato numerico personalizzato non è impostato (ad esempio, il formato numerico è incorporato), verrà restituita una stringa vuota "". |
| [Font](../../aspose.cells.griddesktop/style/font/) { get; set; } | Ottiene un oggetto [`GridFont`](../../aspose.cells.griddesktop.data/gridfont/). |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor/) { get; set; } | Ottiene o imposta il colore di primo piano di uno stile. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment/) { get; set; } | Ottiene o imposta l'attributo di allineamento orizzontale. |
| [Indent](../../aspose.cells.griddesktop/style/indent/) { get; set; } | Rappresenta il livello m_IndentLevel per la cella o l'intervallo. Può essere solo un intero da 0 a 15. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype/) { get; set; } | Ottiene o imposta il formato di visualizzazione di numeri e date. I modelli di formattazione sono diversi per le varie regioni. |
| [Pattern](../../aspose.cells.griddesktop/style/pattern/) { get; set; } | Ottiene o imposta il tipo di modello di sfondo della cella. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation/) { get; set; } | Rappresenta l'angolo di rotazione del testo. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink/) { get; set; } | Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza della colonna disponibile. |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection/) { get; set; } | Ottiene o imposta l'attributo di direzione del testo. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped/) { get; set; } | Ottiene o imposta un valore che indica se il testo all'interno di una cella è a capo. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment/) { get; set; } | Ottiene o imposta l'attributo di allineamento verticale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone/)() | Crea e restituisce una copia di questo oggetto. **NOTE:** Se cloni uno stile con nome, il nome non viene clonato perché il nome dello stile deve essere unico. Pertanto, lo stile clonato non sarà "equals to" lo stile originale. |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor/)(BorderType, Color) | Imposta il colore del bordo specificato. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline/)(BorderType, BorderLineType) | Imposta il tipo di linea del bordo specificato. |

### Vedi anche

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


