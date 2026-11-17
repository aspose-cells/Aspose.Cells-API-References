---
title: "SvgImageOptions Classe"
linktitle: "SvgImageOptions"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "SvgImageOptions classe. Incapsula l'oggetto che rappresenta svgimageoptions in Go."
type: docs
weight: 200
url: /it/go-cpp/svgimageoptions/
---

## SvgImageOptions class

Opzioni per generare un'immagine SVG.

```go

type SvgImageOptions struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewSvgImageOptions](./newsvgimageoptions/) | Costruttore. |
| [NewSvgImageOptions_ImageOrPrintOptions](./newsvgimageoptions_imageorprintoptions/) | Costruisce da un oggetto genitore. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetImageType](./getimagetype/) | Ottiene o imposta il formato delle immagini generate.valore predefinito: PNG. |
| [SetImageType](./setimagetype/) | Ottiene o imposta il formato delle immagini generate.valore predefinito: PNG. |
| [GetFitToViewPort](./getfittoviewport/) | se questa proprietà è true, l'svg generato si adatterà alla viewport. |
| [SetFitToViewPort](./setfittoviewport/) | se questa proprietà è true, l'svg generato si adatterà alla viewport. |
| [GetCssPrefix](./getcssprefix/) | Ottiene o imposta il prefisso del nome css in svg,il valore predefinito è una stringa vuota. |
| [SetCssPrefix](./setcssprefix/) | Ottiene o imposta il prefisso del nome css in svg,il valore predefinito è una stringa vuota. |
| [GetEmbeddedFontType](./getembeddedfonttype/) | Ottiene o imposta il tipo di carattere incorporato in Svg. |
| [SetEmbeddedFontType](./setembeddedfonttype/) | Ottiene o imposta il tipo di carattere incorporato in Svg. |
| [SetPrintWithStatusDialog](./setprintwithstatusdialog/) | Se PrintWithStatusDialog = true , verrà mostrata una finestra di dialogo che indica lo stato di stampa corrente.altrimenti non verrà mostrata alcuna finestra di dialogo. |
| [GetPrintWithStatusDialog](./getprintwithstatusdialog/) | Se PrintWithStatusDialog = true , verrà mostrata una finestra di dialogo che indica lo stato di stampa corrente.altrimenti non verrà mostrata alcuna finestra di dialogo. |
| [GetHorizontalResolution](./gethorizontalresolution/) | Ottiene o imposta la risoluzione orizzontale per le immagini generate, in punti per pollice. |
| [SetHorizontalResolution](./sethorizontalresolution/) | Ottiene o imposta la risoluzione orizzontale per le immagini generate, in punti per pollice. |
| [GetVerticalResolution](./getverticalresolution/) | Ottiene o imposta la risoluzione verticale per le immagini generate, in punti per pollice. |
| [SetVerticalResolution](./setverticalresolution/) | Ottiene o imposta la risoluzione verticale per le immagini generate, in punti per pollice. |
| [GetTiffCompression](./gettiffcompression/) | Ottiene o imposta il tipo di compressione da applicare solo quando si salvano pagine nel formato <c>Tiff</c>. |
| [SetTiffCompression](./settiffcompression/) | Ottiene o imposta il tipo di compressione da applicare solo quando si salvano pagine nel formato <c>Tiff</c>. |
| [GetTiffColorDepth](./gettiffcolordepth/) | Ottiene o imposta la profondità di bit da applicare solo quando si salvano pagine nel formato <c>Tiff</c>. |
| [SetTiffColorDepth](./settiffcolordepth/) | Ottiene o imposta la profondità di bit da applicare solo quando si salvano pagine nel formato <c>Tiff</c>. |
| [GetTiffBinarizationMethod](./gettiffbinarizationmethod/) | Ottiene o imposta il metodo usato durante la conversione delle immagini al formato 1 bpp quando ImageType è Tiff e TiffCompression è uguale a Ccitt3 o Ccitt4. |
| [SetTiffBinarizationMethod](./settiffbinarizationmethod/) | Ottiene o imposta il metodo usato durante la conversione delle immagini al formato 1 bpp quando ImageType è Tiff e TiffCompression è uguale a Ccitt3 o Ccitt4. |
| [GetPrintingPage](./getprintingpage/) | Indica quali pagine non verranno stampate. |
| [SetPrintingPage](./setprintingpage/) | Indica quali pagine non verranno stampate. |
| [GetQuality](./getquality/) | Ottiene o imposta un valore che determina la qualità delle immagini generate da applicare solo quando si salvano pagine nel formato <c>Jpeg</c>. Il valore predefinito è 100 |
| [SetQuality](./setquality/) | Ottiene o imposta un valore che determina la qualità delle immagini generate da applicare solo quando si salvano pagine nel formato <c>Jpeg</c>. Il valore predefinito è 100 |
| [GetOnePagePerSheet](./getonepagepersheet/) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta del pagesetup sarà invalida, ma le altre impostazioni del pagesetup continueranno ad avere effetto. |
| [SetOnePagePerSheet](./setonepagepersheet/) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta del pagesetup sarà invalida, ma le altre impostazioni del pagesetup continueranno ad avere effetto. |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | Se AllColumnsInOnePagePerSheet è true , tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato.La larghezza del formato carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup continueranno ad avere effetto. |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | Se AllColumnsInOnePagePerSheet è true , tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato.La larghezza del formato carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup continueranno ad avere effetto. |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [GetOnlyArea](./getonlyarea/) | Se questa proprietà è vera, verrà generata un'Area e nessuna scala avrà effetto. |
| [SetOnlyArea](./setonlyarea/) | Se questa proprietà è vera, verrà generata un'Area e nessuna scala avrà effetto. |
| [GetTransparent](./gettransparent/) | Indica se lo sfondo dell'immagine generata deve essere trasparente. |
| [SetTransparent](./settransparent/) | Indica se lo sfondo dell'immagine generata deve essere trasparente. |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | Indica se sostituire il font del carattere solo quando il font della cella non è compatibile. |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | Indica se sostituire il font del carattere solo quando il font della cella non è compatibile. |
| [SetPageIndex](./setpageindex/) | Ottiene o imposta l'indice basato su zero della prima pagina da salvare. |
| [GetPageIndex](./getpageindex/) | Ottiene o imposta l'indice basato su zero della prima pagina da salvare. |
| [SetPageCount](./setpagecount/) | Ottiene o imposta il numero di pagine da salvare. |
| [GetPageCount](./getpagecount/) | Ottiene o imposta il numero di pagine da salvare. |
| [SetDesiredSize](./setdesiredsize/) | Imposta la larghezza e l'altezza desiderate dell'immagine. |
| [IsOptimized](./isoptimized/) | Indica se ottimizzare gli elementi di output. |
| [SetIsOptimized](./setisoptimized/) | Indica se ottimizzare gli elementi di output. |
| [GetDefaultFont](./getdefaultfont/) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode. |
| [SetDefaultFont](./setdefaultfont/) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per visualizzare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per mostrare questi caratteri Unicode. |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta questo su true per provare a utilizzare prima il font predefinito della cartella di lavoro per visualizzare questi caratteri. |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta questo su true per provare a utilizzare prima il font predefinito della cartella di lavoro per visualizzare questi caratteri. |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [GetGridlineType](./getgridlinetype/) | Ottiene o imposta il tipo di linea della griglia. |
| [SetGridlineType](./setgridlinetype/) | Ottiene o imposta il tipo di linea della griglia. |
| [GetGridlineColor](./getgridlinecolor/) | Ottiene o imposta il colore della griglia. |
| [SetGridlineColor](./setgridlinecolor/) | Ottiene o imposta il colore della griglia. |
| [GetTextCrossType](./gettextcrosstype/) | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera quella della cella. |
| [SetTextCrossType](./settextcrosstype/) | Ottiene o imposta il tipo di visualizzazione del testo quando la larghezza del testo supera quella della cella. |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | Ottiene o imposta la lingua di modifica predefinita. |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | Ottiene o imposta la lingua di modifica predefinita. |
| [GetSheetSet](./getsheetset/) | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: Aspose.Cells.Rendering.SheetSet.Visible. |
| [SetSheetSet](./setsheetset/) | Ottiene o imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: Aspose.Cells.Rendering.SheetSet.Visible. |
| [GetEmfRenderSetting](./getemfrendersetting/) | Impostazione per il rendering dei metafile EMF nel file sorgente. |
| [SetEmfRenderSetting](./setemfrendersetting/) | Impostazione per il rendering dei metafile EMF nel file sorgente. |
| [GetCustomRenderSettings](./getcustomrendersettings/) | Ottiene o imposta le impostazioni personalizzate durante il rendering. |
| [SetCustomRenderSettings](./setcustomrendersettings/) | Ottiene o imposta le impostazioni personalizzate durante il rendering. |
