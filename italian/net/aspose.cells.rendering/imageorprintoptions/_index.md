---
title: ImageOrPrintOptions
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Consente di specificare le opzioni durante il rendering del foglio di lavoro in immagini la stampa del foglio di lavoro o il rendering del grafico in unimmagine.
type: docs
weight: 5140
url: /it/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Consente di specificare le opzioni durante il rendering del foglio di lavoro in immagini, la stampa del foglio di lavoro o il rendering del grafico in un'immagine.

```csharp
public class ImageOrPrintOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | Default_Costruttore |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet) { get; set; } | Se AllColumnsInOnePagePerSheet è true , tutto il contenuto delle colonne di un foglio verrà restituito a una sola pagina nel risultato. La larghezza del formato carta di pagesetup non sarà valida e le altre impostazioni di pagesetup avranno ancora effetto. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont) { get; set; } | Quando i caratteri in Excel sono Unicode e non possono essere impostati con il carattere corretto nello stile della cella, Possono apparire come blocchi in pdf, immagine. Impostalo su true per provare a utilizzare il carattere predefinito della cartella di lavoro per mostrare prima questi caratteri. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler) { get; set; } | Il client può stampare un output speciale sulla stampante quando stampa ogni pagina utilizzando questo EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler) { get; set; } | Il client può controllare l'impostazione della pagina della stampante quando stampa ogni pagina utilizzando questo EventHandler |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage) { get; set; } | Ottiene o imposta la lingua di modifica predefinita. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont) { get; set; } | Quando i caratteri in Excel sono Unicode e non possono essere impostati con il font corretto nello stile della cella, Possono apparire come blocchi in pdf,image. Impostare il DefaultFont come MingLiu o MS Gothic per mostrare questi caratteri. Se questa proprietà è non impostato, Aspose.Cells utilizzerà il carattere predefinito del sistema per mostrare questi caratteri unicode. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler) { get; set; } | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg) { get; set; } | Indica il nome del file dell'immagine incorporata in svg. Questo dovrebbe essere il percorso completo con una directory come "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype) { get; set; } | Ottiene o imposta un EmfType che specifica il formato del Metafile.. Il valore predefinito è EmfPlusDual. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype) { get; set; } | Ottiene o imposta il tipo di griglia. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution) { get; set; } | Ottiene o imposta la risoluzione orizzontale per le immagini generate, in punti per pollice. Applica il metodo di generazione dell'immagine ad eccezione delle immagini in formato Emf. |
| [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype) { get; set; } | Ottiene o imposta il formato delle immagini generate. valore predefinito: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit) { get; set; } | Indica se la larghezza e l'altezza delle celle vengono adattate automaticamente in base al valore della cella. Il valore predefinito è false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity) { get; set; } | Indica se sostituire il font del carattere solo quando il font della cella non è compatibile con esso. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized) { get; set; } | Indica se ottimizzare gli elementi di output. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet) { get; set; } | Se OnePagePerSheet è true , tutto il contenuto di un foglio verrà restituito a una sola pagina nel risultato. Il formato carta di pagesetup non sarà valido e le altre impostazioni di pagesetup avranno ancora effetto. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea) { get; set; } | Se questa proprietà è true , verrà emessa un'area e nessuna scala avrà effetto. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint) { get; set; } | Indica se stampare una pagina vuota quando non c'è nulla da stampare. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount) { get; set; } | Ottiene o imposta il numero di pagine da salvare. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex) { get; set; } | Ottiene o imposta l'indice in base 0 della prima pagina da salvare. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback) { get; set; } | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat) { get; set; } | Ottiene o imposta il formato pixel per le immagini generate. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage) { get; set; } | Indica quali pagine non verranno stampate. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog) { get; set; } | Se PrintWithStatusDialog = true, ci sarà una finestra di dialogo che mostra lo stato di stampa corrente. altrimenti non verrà visualizzata alcuna finestra di dialogo simile. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality) { get; set; } | Ottiene o imposta un valore che determina la qualità delle immagini generate da applicare solo quando si salvano le pagine nel`jpeg` formato. Il valore predefinito è 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat) { get; set; } | Ottiene o imposta il formato del file di output type Support Tiff/XPS |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode) { get; set; } | Specifica se l'arrotondamento (antialias) viene applicato a linee e curve e ai bordi delle aree riempite. Il valore predefinito è SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport) { get; set; } | se questa proprietà è vera, lo svg generato si adatterà alla visualizzazione della porta. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype) { get; set; } | Ottiene o imposta la visualizzazione del tipo di testo quando la larghezza del testo è maggiore della larghezza della cella. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint) { get; set; } | Specifica la qualità del rendering del testo. Il valore predefinito è TextRenderingHint.SystemDefault |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth) { get; set; } | Ottiene o imposta la profondità di bit da applicare solo quando si salvano le pagine nel file`Tiff` formato. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression) { get; set; } | Ottiene o imposta il tipo di compressione da applicare solo quando si salvano le pagine nel file`Tiff` formato. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent) { get; set; } | Indica se lo sfondo dell'immagine generata deve essere trasparente. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution) { get; set; } | Ottiene o imposta la risoluzione verticale per le immagini generate, in punti per pollice. Applica il metodo di generazione dell'immagine tranne l'immagine in formato Emf. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback) { get; set; } | Ottiene o imposta la richiamata di avviso. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize)(int, int) | Imposta la larghezza e l'altezza desiderate dell'immagine. |

### Esempi

```csharp

[C#]

//Imposta le opzioni immagine o stampa
ImageOrPrintOptions options = new ImageOrPrintOptions();

//Imposta il formato dell'immagine di output
options.ImageType = ImageType.Png;

//Imposta la risoluzione orizzontale
options.HorizontalResolution = 300;

//Imposta la risoluzione verticale
options.VerticalResolution = 300;

//Crea cartella di lavoro
Workbook book = new Workbook("test.xls");

//Salva il grafico come immagine utilizzando le opzioni di ImageOrPrint
book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'Imposta le opzioni immagine o stampa
Dim options As New ImageOrPrintOptions()

'Imposta il formato dell'immagine di output
options.ImageType = ImageType.Png

'Imposta la risoluzione orizzontale
options.HorizontalResolution = 300

'Imposta la risoluzione verticale
options.VerticalResolution = 300

'Istanziare cartella di lavoro
Dim book As New Workbook("test.xls")

'Salva il grafico come immagine utilizzando le opzioni di ImageOrPrint
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
