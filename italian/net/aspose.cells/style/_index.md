---
title: "Classe Style"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Style class. Rappresenta lo stile di visualizzazione dei documenti Excel, come colore del carattere, allineamento, bordo, ecc. L'oggetto Style contiene tutti gli attributi di stile, come carattere, formato numerico, allineamento e così via, come proprietà"
type: docs
url: /it/net/aspose.cells/style/
---
## Style class

Rappresenta lo stile di visualizzazione del documento Excel, come font, colore, allineamento, bordo, ecc. L'oggetto Style contiene tutti gli attributi di stile (font, formato numerico, allineamento e così via) come proprietà.

```csharp
public class Style
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Style](style/)() | (**Obsoleto.**) Inizializza una nuova istanza della classe `Style`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor/) { get; set; } | Ottiene e imposta il colore di sfondo con un valore ARGB a 32 bit. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor/) { get; set; } | Ottiene o imposta il colore di sfondo di uno stile. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor/) { get; set; } | Ottiene e imposta il colore del tema di sfondo. |
| [Borders](../../aspose.cells/style/borders/) { get; } | Ottiene la [`BorderCollection`](../bordercollection/) dello stile. |
| [BottomBorder](../../aspose.cells/style/bottomborder/) { get; } | Ottiene il bordo inferiore. |
| [CultureCustom](../../aspose.cells/style/culturecustom/) { get; set; } | Ottiene e imposta la stringa di modello dipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato. |
| [Custom](../../aspose.cells/style/custom/) { get; set; } | Rappresenta la stringa di formato numerico personalizzato di questo oggetto stile. Se il formato numerico personalizzato non è impostato (ad esempio, il formato numerico è incorporato), verrà restituita una stringa vuota "". |
| [Font](../../aspose.cells/style/font/) { get; } | Ottiene un oggetto [`Font`](./font/). |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor/) { get; set; } | Ottiene e imposta il colore di primo piano con un valore ARGB a 32 bit. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor/) { get; set; } | Ottiene o imposta il colore di primo piano di uno stile. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor/) { get; set; } | Ottiene e imposta il colore del tema in primo piano. |
| [HasBorders](../../aspose.cells/style/hasborders/) { get; } | Verifica se sono stati impostati bordi per lo stile. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment/) { get; set; } | Ottiene o imposta il tipo di allineamento orizzontale del testo in una cella. |
| [IndentLevel](../../aspose.cells/style/indentlevel/) { get; set; } | Rappresenta il livello di rientro per la cella o l'intervallo. Può essere solo un intero da 0 a 250. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom/) { get; } | Ottiene la stringa di modello indipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato. |
| [IsAlignmentApplied](../../aspose.cells/style/isalignmentapplied/) { get; set; } | Indica se la formattazione dell'allineamento deve essere applicata. |
| [IsBorderApplied](../../aspose.cells/style/isborderapplied/) { get; set; } | Indica se la formattazione del bordo deve essere applicata. |
| [IsCheckBox](../../aspose.cells/style/ischeckbox/) { get; set; } | Indica se è uno stile di casella di controllo. |
| [IsDateTime](../../aspose.cells/style/isdatetime/) { get; } | Indica se il formato numerico è un formato data. |
| [IsFillApplied](../../aspose.cells/style/isfillapplied/) { get; set; } | Indica se la formattazione di riempimento deve essere applicata. |
| [IsFontApplied](../../aspose.cells/style/isfontapplied/) { get; set; } | Indica se la formattazione del carattere deve essere applicata. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden/) { get; set; } | Rappresenta se la formula sarà nascosta quando il foglio di lavoro è protetto. |
| [IsGradient](../../aspose.cells/style/isgradient/) { get; set; } | Indica se l'ombreggiatura della cella è un modello a gradiente. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed/) { get; set; } | Indica se l'allineamento giustificato o distribuito delle celle deve essere usato sull'ultima riga di testo. |
| [IsLocked](../../aspose.cells/style/islocked/) { get; set; } | Ottiene o imposta un valore che indica se una cella può essere modificata o meno. |
| [IsNumberFormatApplied](../../aspose.cells/style/isnumberformatapplied/) { get; set; } | Indica se la formattazione numerica deve essere applicata. |
| [IsPercent](../../aspose.cells/style/ispercent/) { get; } | Indica se il formato numerico è un formato percentuale. |
| [IsProtectionApplied](../../aspose.cells/style/isprotectionapplied/) { get; set; } | Indica se la formattazione di protezione deve essere applicata. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped/) { get; set; } | Ottiene o imposta un valore che indica se il testo all'interno di una cella è a capo. |
| [LeftBorder](../../aspose.cells/style/leftborder/) { get; } | Ottiene il bordo sinistro. |
| [Name](../../aspose.cells/style/name/) { get; set; } | Ottiene o imposta il nome dello stile. |
| [Number](../../aspose.cells/style/number/) { get; set; } | Ottiene o imposta il formato di visualizzazione di numeri e date. I modelli di formattazione sono diversi per le varie regioni. |
| [ParentStyle](../../aspose.cells/style/parentstyle/) { get; } | Ottiene lo stile genitore di questo stile. |
| [Pattern](../../aspose.cells/style/pattern/) { get; set; } | Ottiene o imposta il tipo di modello di sfondo della cella. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix/) { get; set; } | Indica se il valore della cella inizia con un apostrofo. |
| [RightBorder](../../aspose.cells/style/rightborder/) { get; } | Ottiene il bordo destro. |
| [RotationAngle](../../aspose.cells/style/rotationangle/) { get; set; } | Rappresenta l'angolo di rotazione del testo. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit/) { get; set; } | Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza della colonna disponibile. |
| [TextDirection](../../aspose.cells/style/textdirection/) { get; set; } | Rappresenta l'ordine di lettura del testo. |
| [TopBorder](../../aspose.cells/style/topborder/) { get; } | Ottiene il bordo superiore. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment/) { get; set; } | Ottiene o imposta il tipo di allineamento verticale del testo in una cella. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Copy](../../aspose.cells/style/copy/)(Style) | Copia i dati da un altro oggetto stile |
| override [Equals](../../aspose.cells/style/equals/)(object) | Determina se due istanze di Style sono uguali. |
| override [GetHashCode](../../aspose.cells/style/gethashcode/)() | Funziona come funzione hash per un oggetto Style. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient/)(out Color, out Color, out GradientStyleType, out int) | (**Obsolete.**) Ottieni l'impostazione del gradiente a due colori. |
| [GetTwoColorGradientSetting](../../aspose.cells/style/gettwocolorgradientsetting/)() | Ottieni l'impostazione del gradiente a due colori. |
| [IsModified](../../aspose.cells/style/ismodified/)(StyleModifyFlag) | Verifica se le proprietà specificate dello stile sono state modificate. Utilizzato per lo stile dei ConditionalFormattings per verificare se le proprietà specificate di questo stile devono essere utilizzate quando si applicano i ConditionalFormattings su una cella. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder)(BorderType, CellBorderType, CellsColor) | Imposta i bordi dello stile. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder_1)(BorderType, CellBorderType, Color) | Imposta i bordi dello stile. |
| [SetCustom](../../aspose.cells/style/setcustom/)(string, bool) | Imposta la stringa di formato numerico personalizzato di una cella. |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Imposta i bordi di contorno |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Imposta i bordi di contorno |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor/)(BackgroundType, Color, Color) | Imposta il colore di sfondo. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient/)(Color, Color, GradientStyleType, int) | Imposta il riempimento specificato a un gradiente a due colori. |
| [ToJson](../../aspose.cells/style/tojson/)() | Converti `Style` in dati struct JSON. |
| [Update](../../aspose.cells/style/update/)() | Applica lo stile denominato agli stili delle celle che utilizzano questo stile denominato. Funziona come fare clic sul pulsante "ok" dopo aver terminato la modifica dello stile. Si applica solo agli stili denominati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleDemo
    {
        public static void StyleExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accedi a una cella dal foglio di lavoro
            Cell cell = worksheet.Cells["A1"];
            
            // Ottieni lo stile della cella
            Style style = cell.GetStyle();
            
            // Imposta varie proprietà dello stile
            style.Font.Name = "Times New Roman";
            style.Font.Color = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;
            style.IsLocked = true;
            style.Number = 15; // Date format
            style.IndentLevel = 2;
            style.RotationAngle = 45;
            style.IsFormulaHidden = true;
            style.ShrinkToFit = true;
            style.TextDirection = TextDirectionType.RightToLeft;
            style.IsJustifyDistributed = true;
            style.QuotePrefix = true;
            style.IsGradient = true;
            style.IsNumberFormatApplied = true;
            style.IsFontApplied = true;
            style.IsAlignmentApplied = true;
            style.IsBorderApplied = true;
            style.IsFillApplied = true;
            style.IsProtectionApplied = true;
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.ForegroundArgbColor = Color.Red.ToArgb();
            style.Custom = "0.00%";
            style.CultureCustom = "0.00%";
            
            // Imposta lo stile sulla cella
            cell.SetStyle(style);
            
            // Salva la cartella di lavoro
            workbook.Save("StyleExample.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


