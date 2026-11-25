---
title: "Classe SvgImageOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.SvgImageOptions. Opzioni per generare immagini Svg"
type: docs
url: /it/net/aspose.cells.rendering/svgimageoptions/
---
## SvgImageOptions class

Opzioni per la generazione di un'immagine Svg.

```csharp
public class SvgImageOptions : ImageOrPrintOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SvgImageOptions](svgimageoptions/)() | Ctor. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà emesso su una sola pagina nel risultato. La larghezza della dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup continueranno ad avere effetto. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) Indica il tipo di immagine del grafico durante la conversione. valore predefinito: PNG. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta questo a true per provare a utilizzare il font predefinito della cartella di lavoro per mostrare questi caratteri per primi. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CssPrefix](../../aspose.cells.rendering/svgimageoptions/cssprefix/) { get; set; } | Ottiene e imposta il prefisso del nome CSS in SVG, il valore predefinito è una stringa vuota. |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | Il client può eseguire un output speciale alla stampante quando stampa ogni pagina usando questo EventHandler (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | Il client può controllare le impostazioni di pagina della stampante quando stampa ogni pagina usando questo EventHandler (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | Ottiene o imposta impostazioni personalizzate durante il rendering. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | Ottiene o imposta la lingua di modifica predefinita. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per mostrare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per visualizzare questi caratteri Unicode. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmbeddedFontType](../../aspose.cells.rendering/svgimageoptions/embeddedfonttype/) { get; set; } | Ottiene o imposta il tipo di font incorporato in SVG. |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) Indica il nome file dell'immagine incorporata in SVG. Deve essere un percorso completo con directory, ad esempio "c:\\xpsEmbedded" (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | Impostazione per il rendering dei metafile EMF nel file sorgente. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | Ottiene o imposta un EmfType che specifica il formato del Metafile. Il valore predefinito è EmfPlusDual. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [FitToViewPort](../../aspose.cells.rendering/svgimageoptions/fittoviewport/) { get; set; } | Se questa proprietà è true, l'SVG generato si adatterà alla viewport. |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | Ottiene o imposta il colore della griglia. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | Ottiene o imposta il tipo di linea della griglia. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | Ottiene o imposta la risoluzione orizzontale per le immagini generate, in punti per pollice. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| override [ImageType](../../aspose.cells.rendering/svgimageoptions/imagetype/) { get; set; } | Ottiene o imposta il formato delle immagini generate. valore predefinito: PNG. |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) Indica se la larghezza e l'altezza delle celle vengono adattate automaticamente al valore della cella. Il valore predefinito è false. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | Indica se ottimizzare gli elementi di output. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup continueranno ad avere effetto. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | Se questa proprietà è true, verrà esportata un'Area e nessuna scala avrà effetto. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | Indica se esportare una pagina vuota quando non c'è nulla da stampare. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | Ottiene o imposta il numero di pagine da salvare. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | Ottiene o imposta l'indice basato su zero della prima pagina da salvare. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | Controlla/Indica l'avanzamento del processo di salvataggio delle pagine. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | Ottiene o imposta il formato pixel per le immagini generate. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | Indica quali pagine non saranno stampate. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | Se PrintWithStatusDialog = true, verrà mostrata una finestra di dialogo che indica lo stato di stampa corrente; altrimenti nessuna finestra di dialogo verrà mostrata. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | Ottiene o imposta un valore che determina la qualità delle immagini generate da applicare solo quando si salvano le pagine nel formato `Jpeg`. Il valore predefinito è 100. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) Ottiene o imposta il tipo di formato file di output. Supporta Tiff/XPS. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [`Visible`](../sheetset/visible/). (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | Specifica se l'anti-aliasing è applicato a linee, curve e ai bordi delle aree riempite. Il valore predefinito è SmoothingMode.None. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) Ottiene e imposta il prefisso del nome CSS in SVG, il valore predefinito è una stringa vuota. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) se questa proprietà è true, l'SVG generato si adatterà alla viewport. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera la larghezza della cella. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | Specifica la qualità del rendering del testo. Il valore predefinito è TextRenderingHint.SystemDefault. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | Ottiene o imposta il metodo usato durante la conversione delle immagini al formato 1 bpp quando [`ImageType`](../imageorprintoptions/imagetype/) è Tiff e [`TiffCompression`](../imageorprintoptions/tiffcompression/) è uguale a Ccitt3 o Ccitt4. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | Ottiene o imposta la profondità di bit da applicare solo quando si salvano le pagine nel formato `Tiff`. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | Ottiene o imposta il tipo di compressione da applicare solo quando si salvano le pagine nel formato `Tiff`. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | Indica se lo sfondo dell'immagine generata deve essere trasparente. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | Ottiene o imposta la risoluzione verticale per le immagini generate, in punti per pollice. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | Ottiene o imposta il callback di avviso. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int) | (**Obsolete.**) Imposta la larghezza e l'altezza desiderate dell'immagine. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int, bool) | Imposta la larghezza e l'altezza desiderate dell'immagine. (Ereditato da [`ImageOrPrintOptions`](../imageorprintoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgImageOptionsDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Popola dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(12000);
            worksheet.Cells["A3"].PutValue(16500);
            worksheet.Cells["B1"].PutValue("Q2");
            worksheet.Cells["B2"].PutValue(25500);
            worksheet.Cells["B3"].PutValue(10800);

            // Crea un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // Inizializza le opzioni immagine SVG
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // Configura le opzioni di rendering SVG
            svgOptions.FitToViewPort = true;
            svgOptions.CssPrefix = "chart-";
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
            svgOptions.ImageType = ImageType.Svg;

            // Imposta la qualità di stampa e la risoluzione
            svgOptions.PrintWithStatusDialog = true;
            svgOptions.HorizontalResolution = 300;
            svgOptions.VerticalResolution = 300;

            // Renderizza il grafico in SVG con le opzioni configurate
            chart.ToImage("chart_output.svg", svgOptions);

            // Dimostra l'integrazione del salvataggio della cartella di lavoro
            workbook.Save("SvgRenderingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../imageorprintoptions/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


