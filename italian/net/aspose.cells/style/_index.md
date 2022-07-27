---
title: Style
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta lo stile di visualizzazione del documento Excel come font colore allineamento bordo ecc. Loggetto Stile contiene tutti gli attributi di stile carattere formato numerico allineamento e così via come proprietà.
type: docs
weight: 5750
url: /it/net/aspose.cells/style/
---
## Style class

Rappresenta lo stile di visualizzazione del documento Excel, come font, colore, allineamento, bordo, ecc. L'oggetto Stile contiene tutti gli attributi di stile (carattere, formato numerico, allineamento e così via) come proprietà.

```csharp
public class Style
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | Ottiene e imposta il colore di sfondo con un valore ARGB a 32 bit. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | Ottiene o imposta il colore di sfondo di uno stile. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | Ottiene e imposta il colore del tema di sfondo. |
| [Borders](../../aspose.cells/style/borders) { get; } | Ottiene il[`BorderCollection`](../bordercollection) dello stile. |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | Ottiene e imposta la stringa del modello dipendente dalle impostazioni cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa del modello corrispondente al numero incorporato. |
| [Custom](../../aspose.cells/style/custom) { get; set; } | Rappresenta la stringa del formato del numero personalizzato di questo oggetto di stile. Se il formato del numero personalizzato non è impostato (ad esempio, il formato del numero è incorporato), verrà restituito "". |
| [Font](../../aspose.cells/style/font) { get; } | Ottiene a[`Font`](./font) oggetto. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | Ottiene e imposta il colore di primo piano con un valore ARGB a 32 bit. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | Ottiene o imposta il colore di primo piano di uno stile. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | Ottiene e imposta il colore del tema in primo piano. |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | Verifica se sono stati impostati dei bordi per lo stile. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | Ottiene o imposta il tipo di allineamento orizzontale del testo in una cella. |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | Rappresenta il livello di rientro per la cella o l'intervallo. Può essere solo un numero intero compreso tra 0 e 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | Ottiene la stringa del modello indipendente dalle impostazioni cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa del modello corrispondente al numero incorporato. |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | Indica se il formato del numero è un formato data. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | Indica se la formula sarà nascosta quando il foglio di lavoro è protetto. |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | Indica se l'ombreggiatura della cella è un motivo sfumato. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | Indica se le celle giustificate o l'allineamento distribuito devono essere utilizzate sull'ultima riga di testo. |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | Ottiene o imposta un valore che indica se una cella può essere modificata o meno. |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | Indica se il formato numerico è un formato percentuale. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | Ottiene o imposta un valore che indica se il testo all'interno di una cella è a capo. |
| [Name](../../aspose.cells/style/name) { get; set; } | Ottiene o imposta il nome dello stile. |
| [Number](../../aspose.cells/style/number) { get; set; } | Ottiene o imposta il formato di visualizzazione di numeri e date. I modelli di formattazione sono diversi per le diverse regioni. |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | Ottiene lo stile padre di questo stile. |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | Ottiene o imposta il tipo di motivo di sfondo della cella. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | Indica se il valore della cella inizia con virgolette singole. |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | Rappresenta l'angolo di rotazione del testo. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | Indica se il testo si riduce automaticamente per adattarsi alla larghezza della colonna disponibile. |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | Rappresenta l'ordine di lettura del testo. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | Ottiene o imposta il tipo di allineamento verticale del testo in una cella. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | Copia i dati da un altro oggetto di stile |
| override [Equals](../../aspose.cells/style/equals)(object) | Determina se due istanze di stile sono uguali. |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | Serve come funzione hash per un oggetto Style. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | Ottieni l'impostazione del gradiente a due colori. |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | Verifica se le proprietà specificate dello stile sono state modificate. Utilizzato per lo stile di ConditionalFormattings per verificare se le proprietà specificate di questo stile devono essere utilizzate quando si applicano ConditionalFormattings a una cella. |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | Imposta i bordi dello stile. |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | Imposta la stringa di formato numero personalizzato di una cella. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | Imposta il colore di sfondo. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | Imposta il riempimento specificato su una sfumatura a due colori. |
| [Update](../../aspose.cells/style/update)() | Applica lo stile con nome agli stili delle celle che usano questo stile con nome. Funziona come fare clic sul pulsante "ok" dopo aver finito di modificare lo stile. Si applica solo per lo stile con nome. |

### Esempi

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
