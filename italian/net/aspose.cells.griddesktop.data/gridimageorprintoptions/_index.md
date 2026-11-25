---
title: "Classe GridImageOrPrintOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridDesktop.Data.GridImageOrPrintOptions. Consente di specificare opzioni durante il rendering del foglio di lavoro in immagini, la stampa del foglio di lavoro o il rendering di un grafico in immagine"
type: docs
url: /it/net/aspose.cells.griddesktop.data/gridimageorprintoptions/
---
## GridImageOrPrintOptions class

Consente di specificare le opzioni durante il rendering del foglio di lavoro in immagini, la stampa del foglio di lavoro o il rendering del grafico in immagine.

```csharp
public class GridImageOrPrintOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridImageOrPrintOptions](gridimageorprintoptions/)() | La costruzione di GridImageOrPrintOptions |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà output su una sola pagina nel risultato. La larghezza della dimensione della carta del pagesetup sarà invalida, e le altre impostazioni del pagesetup continueranno ad avere effetto. |
| [CheckWorkbookDefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per visualizzare prima questi caratteri. |
| [DefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/defaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode. |
| [EmbededImageNameInSvg](../../aspose.cells.griddesktop.data/gridimageorprintoptions/embededimagenameinsvg/) { get; set; } | Indica il nome file dell'immagine incorporata in SVG. Deve essere un percorso completo con directory, ad esempio "c:\\xpsEmbedded" |
| [EmfType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/emftype/) { get; set; } | Ottiene o imposta un EmfType che specifica il formato del Metafile. Il valore predefinito è EmfPlusDual. |
| [GridlineType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/gridlinetype/) { get; set; } | Ottiene o imposta il tipo di griglia. |
| [HorizontalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/horizontalresolution/) { get; set; } | Ottiene o imposta la risoluzione orizzontale per le immagini generate, in punti per pollice. Si applica al metodo di generazione dell'immagine, eccetto le immagini in formato EMF. |
| [ImageType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/imagetype/) { get; set; } | Ottiene o imposta il formato delle immagini generate. valore predefinito: PNG. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. |
| [IsOptimized](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isoptimized/) { get; set; } | Indica se ottimizzare gli elementi di output. |
| [OnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onepagepersheet/) { get; set; } | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. Il formato carta di pagesetup sarà invalido, ma le altre impostazioni di pagesetup continueranno ad avere effetto. |
| [OnlyArea](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onlyarea/) { get; set; } | Se questa proprietà è true, verrà output una sola Area e nessuna scala avrà effetto. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [PageCount](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pagecount/) { get; set; } | Ottiene o imposta il numero di pagine da salvare. |
| [PageIndex](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pageindex/) { get; set; } | Ottiene o imposta l'indice basato su 0 della prima pagina da salvare. |
| [PixelFormat](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pixelformat/) { get; set; } | Ottiene o imposta il formato pixel per le immagini generate. |
| [PrintingPage](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printingpage/) { get; set; } | Indica quali pagine non saranno stampate. |
| [PrintWithStatusDialog](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printwithstatusdialog/) { get; set; } | Se PrintWithStatusDialog = true, verrà mostrata una finestra di dialogo che indica lo stato di stampa corrente; altrimenti non verrà mostrata alcuna finestra di dialogo. |
| [Quality](../../aspose.cells.griddesktop.data/gridimageorprintoptions/quality/) { get; set; } | Ottiene o imposta un valore che determina la qualità delle immagini generate da applicare solo quando si salvano le pagine nel formato `Jpeg`. Il valore predefinito è 100 |
| [SmoothingMode](../../aspose.cells.griddesktop.data/gridimageorprintoptions/smoothingmode/) { get; set; } | Specifica se la smussatura (anti-aliasing) viene applicata a linee e curve e ai bordi delle aree riempite. Il valore predefinito è SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.griddesktop.data/gridimageorprintoptions/svgfittoviewport/) { get; set; } | Se questa proprietà è true, l'SVG generato si adatterà alla viewport. |
| [TextCrossType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textcrosstype/) { get; set; } | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera quella della cella. |
| [TextRenderingHint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textrenderinghint/) { get; set; } | Specifica la qualità del rendering del testo. Il valore predefinito è TextRenderingHint.SystemDefault |
| [Transparent](../../aspose.cells.griddesktop.data/gridimageorprintoptions/transparent/) { get; set; } | Indica se lo sfondo dell'immagine generata deve essere trasparente. |
| [VerticalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/verticalresolution/) { get; set; } | Ottiene o imposta la risoluzione verticale per le immagini generate, in punti per pollice. Si applica al metodo di generazione dell'immagine, eccetto le immagini in formato EMF. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setdesiredsize/)(int, int) | Imposta la larghezza e l'altezza desiderate dell'immagine. |
| [setRenderSheetSet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setrendersheetset/)(int[]) | Imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro. Indici dei fogli basati su zero. |

### Vedi anche

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


