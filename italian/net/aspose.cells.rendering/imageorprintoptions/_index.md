---
title: "Classe ImageOrPrintOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.ImageOrPrintOptions. Consente di specificare le opzioni durante il rendering del foglio di lavoro in immagini, la stampa del foglio di lavoro o il rendering del grafico in immagine"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

Consente di specificare le opzioni durante il rendering del foglio di lavoro in immagini, la stampa del foglio di lavoro o il rendering del grafico in immagine.

```csharp
public class ImageOrPrintOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions/)() | Ctor. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà output su una sola pagina nel risultato. La larghezza della dimensione della carta del pagesetup sarà invalida, e le altre impostazioni del pagesetup continueranno ad avere effetto. |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Indica il tipo di immagine del grafico durante la conversione. valore predefinito: PNG. |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per visualizzare prima questi caratteri. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Il client può inviare output speciale alla stampante quando stampa ogni pagina utilizzando questo EventHandler |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Il client può controllare le impostazioni di pagina della stampante quando stampa ogni pagina utilizzando questo EventHandler |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Ottiene o imposta le impostazioni personalizzate durante il rendering. |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Ottiene o imposta la lingua di modifica predefinita. |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf, immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode. |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Indica il nome file dell'immagine incorporata in SVG. Deve essere un percorso completo con directory, ad esempio "c:\\xpsEmbedded" |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Impostazione per il rendering dei metafile EMF nel file sorgente. |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Ottiene o imposta un EmfType che specifica il formato del Metafile. Il valore predefinito è EmfPlusDual. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Ottiene o imposta il colore della griglia. |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Ottiene o imposta il tipo di griglia. |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Ottiene o imposta la risoluzione orizzontale per le immagini generate, in punti per pollice. |
| virtual [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype/) { get; set; } | Ottiene o imposta il formato delle immagini generate. valore predefinito: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Indica se la larghezza e l'altezza delle celle vengono adattate automaticamente al valore della cella. Il valore predefinito è false. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Indica se ottimizzare gli elementi di output. |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. Il formato carta di pagesetup sarà invalido, ma le altre impostazioni di pagesetup continueranno ad avere effetto. |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Se questa proprietà è true, verrà output una sola Area e nessuna scala avrà effetto. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Ottiene o imposta il numero di pagine da salvare. |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Ottiene o imposta l'indice basato su 0 della prima pagina da salvare. |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Ottiene o imposta il formato pixel per le immagini generate. |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Indica quali pagine non saranno stampate. |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Se PrintWithStatusDialog = true, verrà mostrata una finestra di dialogo che indica lo stato di stampa corrente; altrimenti non verrà mostrata alcuna finestra di dialogo. |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Ottiene o imposta un valore che determina la qualità delle immagini generate da applicare solo quando si salvano le pagine nel formato `Jpeg`. Il valore predefinito è 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Ottiene o imposta il tipo di formato file di output. Supporta Tiff/XPS |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../sheetset/visible/). |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Specifica se la smussatura (anti-aliasing) viene applicata a linee e curve e ai bordi delle aree riempite. Il valore predefinito è SmoothingMode.None |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsoleto.**) Ottiene e imposta il prefisso del nome css in svg, il valore predefinito è una stringa vuota. |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsoleto.**) se questa proprietà è true, lo svg generato si adatterà alla viewport. |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera quella della cella. |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Specifica la qualità del rendering del testo. Il valore predefinito è TextRenderingHint.SystemDefault |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Ottiene o imposta il metodo usato durante la conversione delle immagini al formato a 1 bpp quando [`ImageType`](./imagetype/) è Tiff e [`TiffCompression`](./tiffcompression/) è uguale a Ccitt3 o Ccitt4. |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Ottiene o imposta la profondità di bit da applicare solo quando si salvano le pagine nel formato `Tiff`. |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Ottiene o imposta il tipo di compressione da applicare solo quando si salvano le pagine nel formato `Tiff`. |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Indica se lo sfondo dell'immagine generata deve essere trasparente. |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Ottiene o imposta la risoluzione verticale per le immagini generate, in punti per pollice. |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Ottiene o imposta il callback di avviso. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize)(int, int) | (**Obsoleto.**) Imposta la larghezza e l'altezza desiderate dell'immagine. |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/#setdesiredsize_1)(int, int, bool) | Imposta la larghezza e l'altezza desiderate dell'immagine. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class RenderingClassImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Crea ImageOrPrintOptions e imposta le proprietà
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;

            // Crea una nuova cartella di lavoro con dati di esempio e grafico
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Salva il grafico come immagine usando le opzioni
            chart.ToImage("output_chart.png", options);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


