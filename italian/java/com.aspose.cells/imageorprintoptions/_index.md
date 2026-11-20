---
title: "ImageOrPrintOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Consente di specificare le opzioni durante il rendering del foglio di lavoro in immagini, la stampa del foglio di lavoro o il rendering del grafico in immagine."
type: docs
url: /it/java/com.aspose.cells/imageorprintoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImageOrPrintOptions
```

Consente di specificare le opzioni durante il rendering del foglio di lavoro in immagini, la stampa del foglio di lavoro o il rendering del grafico in immagine.

**Example**

```
         //Set Image Or Print Options
         ImageOrPrintOptions options = new ImageOrPrintOptions();
 
         //Set output image format
         options.setImageType(ImageType.PNG);
 
         //Set Horizontal resolution
         options.setHorizontalResolution(300);
 
         //Set Vertical Resolution
         options.setVerticalResolution(300);
 
         //Instantiate Workbook
         Workbook book = new Workbook("test.xls");
 
         //Save chart as Image using ImageOrPrint Options
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.png", options);
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [ImageOrPrintOptions()](#ImageOrPrintOptions--) | Ctor. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. |
| [getChartImageType()](#getChartImageType--) | Indicare il tipo di immagine del grafico durante la conversione. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [getClass()](#getClass--) |  |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Restituisce le impostazioni personalizzate durante il rendering. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Restituisce la lingua di modifica predefinita. |
| [getDefaultFont()](#getDefaultFont--) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | Indicare il nome file dell'immagine incorporata in SVG. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Impostazione per il rendering dei metafile EMF nel file di origine. |
| [getGridlineColor()](#getGridlineColor--) | Restituisce il colore della linea della griglia. |
| [getGridlineType()](#getGridlineType--) | Restituisce il tipo di griglia. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Restituisce la risoluzione orizzontale per le immagini generate, in punti per pollice. |
| [getImageType()](#getImageType--) | Restituisce il formato delle immagini generate. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. |
| [getOnlyArea()](#getOnlyArea--) | Se questa proprietà è vera, verrà generata un'area e nessuna scala avrà effetto. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [getPageCount()](#getPageCount--) | Restituisce il numero di pagine da salvare. |
| [getPageIndex()](#getPageIndex--) | Restituisce l'indice basato su 0 della prima pagina da salvare. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | Se PrintWithStatusDialog = true, verrà visualizzata una finestra di dialogo che mostra lo stato di stampa corrente. |
| [getPrintingPage()](#getPrintingPage--) | Indica quali pagine non verranno stampate. |
| [getQuality()](#getQuality--) | Restituisce un valore che determina la qualità delle immagini generate da applicare solo quando si salvano le pagine nel formato `Jpeg`. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | Se questa proprietà è vera, l'SVG generato si adatterà alla viewport. |
| [getSaveFormat()](#getSaveFormat--) | Restituisce il tipo di formato file di output. Supporta Tiff/XPS. |
| [getSheetSet()](#getSheetSet--) | Ottiene i fogli da renderizzare. |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | Restituisce il prefisso del nome CSS in SVG; il valore predefinito è una stringa vuota. |
| [getTextCrossType()](#getTextCrossType--) | Ottiene il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella. |
| [getTiffColorDepth()](#getTiffColorDepth--) | Restituisce la profondità di bit da applicare solo quando si salvano le pagine nel formato `Tiff`. |
| [getTiffCompression()](#getTiffCompression--) | Restituisce il tipo di compressione da applicare solo quando si salvano le pagine nel formato `Tiff`. |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | Restituisce il tipo di PhotometricInterpretation da applicare solo quando si salvano le pagine nel formato `Tiff`. |
| [getTransparent()](#getTransparent--) | Indica se lo sfondo dell'immagine generata deve essere trasparente. |
| [getVerticalResolution()](#getVerticalResolution--) | Restituisce la risoluzione verticale per le immagini generate, in punti per pollice. |
| [getWarningCallback()](#getWarningCallback--) | Ottiene il callback di avviso. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | Indica se la larghezza e l'altezza delle celle vengono adattate automaticamente al valore della cella. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. |
| [isOptimized()](#isOptimized--) | Indica se ottimizzare gli elementi di output. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | Indica se la larghezza e l'altezza delle celle vengono adattate automaticamente al valore della cella. |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | Indicare il tipo di immagine del grafico durante la conversione. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Imposta le impostazioni personalizzate durante il rendering. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Imposta la lingua di modifica predefinita. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in pdf,image. |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | Imposta la larghezza e l'altezza desiderate dell'immagine. |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | Imposta la larghezza e l'altezza desiderate dell'immagine. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | Indicare il nome file dell'immagine incorporata in SVG. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Impostazione per il rendering dei metafile EMF nel file di origine. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indica se sostituire solo il font del carattere quando il font della cella non è compatibile. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Imposta il colore della linea della griglia. |
| [setGridlineType(int value)](#setGridlineType-int-) | Imposta il tipo di linea della griglia. |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | Imposta la risoluzione orizzontale per le immagini generate, in punti per pollice. |
| [setImageType(int value)](#setImageType-int-) | Imposta il formato delle immagini generate. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | Se questa proprietà è vera, verrà generata un'area e nessuna scala avrà effetto. |
| [setOptimized(boolean value)](#setOptimized-boolean-) | Indica se ottimizzare gli elementi di output. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indica se generare una pagina vuota quando non c'è nulla da stampare. |
| [setPageCount(int value)](#setPageCount-int-) | Imposta il numero di pagine da salvare. |
| [setPageIndex(int value)](#setPageIndex-int-) | Imposta l'indice basato su zero della prima pagina da salvare. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | Se PrintWithStatusDialog = true, verrà visualizzata una finestra di dialogo che mostra lo stato di stampa corrente. |
| [setPrintingPage(int value)](#setPrintingPage-int-) | Indica quali pagine non verranno stampate. |
| [setQuality(int value)](#setQuality-int-) | Imposta un valore che determina la qualità delle immagini generate da applicare solo quando si salvano le pagine nel formato `Jpeg`. |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | Imposta il valore di una singola preferenza per gli algoritmi di rendering. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | Se questa proprietà è vera, l'SVG generato si adatterà alla viewport. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Imposta il tipo di formato del file di output, supporta Tiff/XPS. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Imposta i fogli da rendere. |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | Imposta il prefisso del nome CSS in SVG; il valore predefinito è una stringa vuota. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Imposta il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella. |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | Imposta la profondità di bit da applicare solo quando si salvano le pagine nel formato `Tiff`. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Imposta il tipo di compressione da applicare solo quando si salvano le pagine nel formato `Tiff`. |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | Imposta il tipo di PhotometricInterpretation da applicare solo quando si salvano le pagine nel formato `Tiff`. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indica se lo sfondo dell'immagine generata deve essere trasparente. |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | Imposta la risoluzione verticale per le immagini generate, in punti per pollice. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Imposta la callback di avviso. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImageOrPrintOptions() {#ImageOrPrintOptions--}
```
public ImageOrPrintOptions()
```


Ctor.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza della dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup avranno comunque effetto.

**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```


Indica il tipo di immagine del grafico durante la conversione. valore predefinito: PNG.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, Chart e Shape vengono sempre renderizzati come elementi vettoriali (ad es. punto, linea) per la qualità del rendering. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per mostrare questi caratteri prima.

**Remarks**

Il valore predefinito è true.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


Restituisce le impostazioni personalizzate durante il rendering.

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Restituisce la lingua di modifica predefinita.

Vedi [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Può visualizzare/renderizzare layout diversi per i paragrafi di testo quando sono impostate lingue di modifica differenti. Il valore predefinito è [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per mostrare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per visualizzare questi caratteri Unicode.

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


Indica il nome file dell'immagine incorporata in svg. Questo dovrebbe essere il percorso completo con directory, ad esempio "c:\\\\xpsEmbedded"

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, rimuovi questa proprietà perché le immagini sono ora sempre incorporate in Svg con formato base64. Questa proprietà sarà rimossa 12 mesi dopo, a partire da aprile 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


Impostazione per il rendering dei metafile EMF nel file di origine.

Vedi [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

I file metafile EMF identificati come "EMF+ Dual" possono contenere sia record EMF+ sia record EMF. Entrambi i tipi di record possono essere usati per renderizzare l'immagine, solo record EMF+, o solo record EMF. Quando [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) è impostato, i record EMF+ verranno analizzati durante il rendering dell'immagine, altrimenti verranno analizzati solo i record EMF. Il valore predefinito è [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). Per i framework che dipendono da .NET System.Drawing.Common, questa impostazione viene ignorata.

**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


Restituisce il colore della linea della griglia.

**Remarks**

Ignorerà le impostazioni del colore delle linee della griglia nel file di origine.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Restituisce il tipo di griglia.

Vedi [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Il valore predefinito è il tipo Dotted.

**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


Restituisce la risoluzione orizzontale per le immagini generate, in punti per pollice.

**Remarks**

Il valore predefinito è 96. Impostare  e  influisce sulla larghezza e altezza dell'immagine di output in pixel.

**Example**

Il codice seguente imposta la risoluzione a 192, la larghezza e l'altezza dell'immagine generata sono il doppio rispetto a quella con la risoluzione lasciata al valore predefinito 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render worksheet page to image.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), opts);
         sr.toImage(0, "Sheet_Page1.png");
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


Ottiene il formato delle immagini generate. valore predefinito: PNG.

Vedi [ImageType](../../com.aspose.cells/imagetype).

**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup continueranno ad avere effetto.

**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```


Se questa proprietà è vera, verrà generata un'area e nessuna scala avrà effetto.

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Indica se generare una pagina vuota quando non c'è nulla da stampare.

**Remarks**

Il valore predefinito è false.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Restituisce il numero di pagine da salvare.

**Remarks**

Il valore predefinito è System.Int32.MaxValue, il che significa che tutte le pagine saranno renderizzate.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Restituisce l'indice basato su 0 della prima pagina da salvare.

**Remarks**

Il valore predefinito è 0.

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


Controlla/Indica l'avanzamento del processo di salvataggio della pagina.

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```


Se PrintWithStatusDialog = true, verrà mostrata una finestra di dialogo che indica lo stato di stampa corrente; altrimenti non verrà mostrata alcuna finestra di dialogo.

**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```


Indica quali pagine non verranno stampate.

Vedi [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


Ottiene un valore che determina la qualità delle immagini generate da applicare solo durante il salvataggio delle pagine nel formato `Jpeg`. Il valore predefinito è 100

**Remarks**

Ha effetto solo durante il salvataggio in JPEG. Il valore deve essere compreso tra 0 e 100. Il valore predefinito è 100.

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


Se questa proprietà è vera, l'SVG generato si adatterà alla viewport.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Questa proprietà sarà rimossa tra 12 mesi a partire da aprile 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Restituisce il tipo di formato file di output. Supporta Tiff/XPS.

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, per Tiff/Svg, utilizzare [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); per Xps, utilizzare [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) con [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Ottiene i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nel workbook: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Il set è ignorato quando viene utilizzato in [SheetRender](../../com.aspose.cells/sheetrender)

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```


Restituisce il prefisso del nome CSS in SVG; il valore predefinito è una stringa vuota.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Questa proprietà sarà rimossa tra 12 mesi a partire da aprile 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Ottiene il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella.

Vedi [TextCrossType](../../com.aspose.cells/textcrosstype).

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


Restituisce la profondità di bit da applicare solo quando si salvano le pagine nel formato `Tiff`.

Vedi [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Ha effetto solo durante il salvataggio in TIFF. Se TiffCompression è impostato su CCITT3 o CCITT4, questo non avrà effetto; la profondità di bit dell'immagine TIFF generata sarà sempre 1.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


Restituisce il tipo di compressione da applicare solo quando si salvano le pagine nel formato `Tiff`.

Vedi [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Ha effetto solo durante il salvataggio in TIFF. Il valore predefinito è Lzw.

**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```


Restituisce il tipo di PhotometricInterpretation da applicare solo quando si salvano le pagine nel formato `Tiff`.

**Remarks**

Ha effetto solo durante il salvataggio in TIFF. Il valore predefinito è -1, indica che non viene applicata alcuna PhotometricInterpretation.

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


Indica se lo sfondo dell'immagine generata deve essere trasparente.

**Remarks**

Il valore predefinito è false. Ciò significa che lo sfondo delle immagini generate è bianco.

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


Restituisce la risoluzione verticale per le immagini generate, in punti per pollice.

**Remarks**

Il valore predefinito è 96. Impostare  e  influisce sulla larghezza e altezza dell'immagine di output in pixel.

**Example**

Il codice seguente imposta la risoluzione a 192, la larghezza e l'altezza dell'immagine generata sono il doppio rispetto a quella con la risoluzione lasciata al valore predefinito 96.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render Chart to image.
         wb.getWorksheets().get(0).getCharts().get(0).toImage("Chart.png", opts);
```

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Ottiene il callback di avviso.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellAutoFit() {#isCellAutoFit--}
```
public boolean isCellAutoFit()
```


Indica se la larghezza e l'altezza delle celle vengono adattate automaticamente al valore della cella. Il valore predefinito è false.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, questa proprietà non è più utilizzata, si prega di rimuovere questa proprietà. Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Indica se sostituire solo il font del carattere quando il font della cella non è compatibile.

**Remarks**

Il valore predefinito è false. Proveremo prima il font predefinito di Workbook e PdfSaveOption/system per il font delle celle.

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


Indica se ottimizzare gli elementi di output.

**Remarks**

Il valore predefinito è false. Attualmente, quando questa proprietà è impostata su true, verranno eseguite le seguenti ottimizzazioni: 1. ottimizzare le linee di bordo. 2. ottimizzare la dimensione del file durante il rendering in immagine Svg.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


Se AllColumnsInOnePagePerSheet è true, tutto il contenuto delle colonne di un foglio verrà esportato in una sola pagina nel risultato. La larghezza della dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup avranno comunque effetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```


Indica se la larghezza e l'altezza delle celle vengono adattate automaticamente al valore della cella. Il valore predefinito è false.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, questa proprietà non è più utilizzata, si prega di rimuovere questa proprietà. Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```


Indica il tipo di immagine del grafico durante la conversione. valore predefinito: PNG.

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, Chart e Shape vengono sempre renderizzati come elementi vettoriali (ad es. punto, linea) per la qualità del rendering. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta questo su true per provare a utilizzare il font predefinito della cartella di lavoro per mostrare questi caratteri prima.

**Remarks**

Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


Imposta le impostazioni personalizzate durante il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


Imposta la lingua di modifica predefinita.

Vedi [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).

**Remarks**

Può visualizzare/renderizzare layout diversi per i paragrafi di testo quando sono impostate lingue di modifica differenti. Il valore predefinito è [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


Quando i caratteri in Excel sono Unicode e non sono impostati con il font corretto nello stile della cella, possono apparire come blocchi in PDF o immagine. Imposta il DefaultFont, ad esempio MingLiu o MS Gothic, per mostrare questi caratteri. Se questa proprietà non è impostata, Aspose.Cells utilizzerà il font predefinito del sistema per visualizzare questi caratteri Unicode.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


Imposta la larghezza e l'altezza desiderate dell'immagine.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) impostando il parametro keepAspectRatio su false. Questa proprietà sarà rimossa tra 12 mesi a partire da maggio 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| desiredWidth | int | larghezza desiderata in pixel |
| desiredHeight | int | altezza desiderata in pixel |

### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```


Imposta la larghezza e l'altezza desiderate dell'immagine.

**Remarks**

La larghezza e l'altezza dell'immagine di output in pixel saranno basate solo sulla larghezza e altezza desiderate impostate. I  e  non influenzeranno la larghezza e l'altezza dell'immagine di output in questo caso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| desiredWidth | int | larghezza desiderata in pixel |
| desiredHeight | int | altezza desiderata in pixel |
| keepAspectRatio | boolean | se mantenere il rapporto d'aspetto dell'immagine originale |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```


Indica il nome file dell'immagine incorporata in svg. Questo dovrebbe essere il percorso completo con directory, ad esempio "c:\\\\xpsEmbedded"

**Remarks**

NOTE: Questo membro è ora obsoleto. Invece, rimuovi questa proprietà perché le immagini sono ora sempre incorporate in Svg con formato base64. Questa proprietà sarà rimossa 12 mesi dopo, a partire da aprile 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


Impostazione per il rendering dei metafile EMF nel file di origine.

Vedi [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).

**Remarks**

I file metafile EMF identificati come "EMF+ Dual" possono contenere sia record EMF+ sia record EMF. Entrambi i tipi di record possono essere usati per renderizzare l'immagine, solo record EMF+, o solo record EMF. Quando [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) è impostato, i record EMF+ verranno analizzati durante il rendering dell'immagine, altrimenti verranno analizzati solo i record EMF. Il valore predefinito è [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). Per i framework che dipendono da .NET System.Drawing.Common, questa impostazione viene ignorata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


Indica se sostituire solo il font del carattere quando il font della cella non è compatibile.

**Remarks**

Il valore predefinito è false. Proveremo prima il font predefinito di Workbook e PdfSaveOption/system per il font delle celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


Imposta il colore della linea della griglia.

**Remarks**

Ignorerà le impostazioni del colore delle linee della griglia nel file di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


Imposta il tipo di linea della griglia.

Vedi [GridlineType](../../com.aspose.cells/gridlinetype).

**Remarks**

Il valore predefinito è il tipo Dotted.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```


Imposta la risoluzione orizzontale per le immagini generate, in punti per pollice.

**Remarks**

Il valore predefinito è 96. Impostare  e  influisce sulla larghezza e altezza dell'immagine di output in pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```


Imposta il formato delle immagini generate. valore predefinito: PNG.

Vedi [ImageType](../../com.aspose.cells/imagetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


Se OnePagePerSheet è true, tutto il contenuto di un foglio verrà esportato in una sola pagina nel risultato. La dimensione della carta di pagesetup sarà invalida, e le altre impostazioni di pagesetup continueranno ad avere effetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```


Se questa proprietà è vera, verrà generata un'area e nessuna scala avrà effetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```


Indica se ottimizzare gli elementi di output.

**Remarks**

Il valore predefinito è false. Attualmente, quando questa proprietà è impostata su true, verranno eseguite le seguenti ottimizzazioni: 1. ottimizzare le linee di bordo. 2. ottimizzare la dimensione del file durante il rendering in immagine Svg.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


Indica se generare una pagina vuota quando non c'è nulla da stampare.

**Remarks**

Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


Imposta il numero di pagine da salvare.

**Remarks**

Il valore predefinito è System.Int32.MaxValue, il che significa che tutte le pagine saranno renderizzate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


Imposta l'indice basato su zero della prima pagina da salvare.

**Remarks**

Il valore predefinito è 0.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


Controlla/Indica l'avanzamento del processo di salvataggio della pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```


Se PrintWithStatusDialog = true, verrà mostrata una finestra di dialogo che indica lo stato di stampa corrente; altrimenti non verrà mostrata alcuna finestra di dialogo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```


Indica quali pagine non verranno stampate.

Vedi [PrintingPageType](../../com.aspose.cells/printingpagetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```


Imposta un valore che determina la qualità delle immagini generate da applicare solo durante il salvataggio delle pagine nel formato `Jpeg`. Il valore predefinito è 100

**Remarks**

Ha effetto solo durante il salvataggio in JPEG. Il valore deve essere compreso tra 0 e 100. Il valore predefinito è 100.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```


Imposta il valore di una singola preferenza per gli algoritmi di rendering. Le categorie di suggerimento includono controlli per la qualità del rendering e il compromesso complessivo tempo/qualità nel processo di rendering. Fare riferimento alla classe RenderingHints per le definizioni di alcune chiavi e valori comuni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| chiave | java.awt.RenderingHints.Key | la chiave del suggerimento da impostare. |
| valore | java.lang.Object | il valore che indica le preferenze per la categoria di suggerimento specificata. |

### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```


Se questa proprietà è vera, l'SVG generato si adatterà alla viewport.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). Questa proprietà sarà rimossa tra 12 mesi a partire da aprile 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Imposta il tipo di formato del file di output, supporta Tiff/XPS.

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, per Tiff/Svg, utilizzare [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); per Xps, utilizzare [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) con [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2022. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


Imposta i fogli da renderizzare. L'impostazione predefinita è tutti i fogli visibili nella cartella di lavoro: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).

**Remarks**

Il set è ignorato quando viene utilizzato in [SheetRender](../../com.aspose.cells/sheetrender)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```


Imposta il prefisso del nome CSS in SVG; il valore predefinito è una stringa vuota.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). Questa proprietà sarà rimossa tra 12 mesi a partire da aprile 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


Imposta il tipo di visualizzazione del testo quando la larghezza del testo è maggiore della larghezza della cella.

Vedi [TextCrossType](../../com.aspose.cells/textcrosstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```


Imposta la profondità di bit da applicare solo quando si salvano le pagine nel formato `Tiff`.

Vedi [ColorDepth](../../com.aspose.cells/colordepth).

**Remarks**

Ha effetto solo durante il salvataggio in TIFF. Se TiffCompression è impostato su CCITT3 o CCITT4, questo non avrà effetto; la profondità di bit dell'immagine TIFF generata sarà sempre 1.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```


Imposta il tipo di compressione da applicare solo quando si salvano le pagine nel formato `Tiff`.

Vedi [TiffCompression](../../com.aspose.cells/tiffcompression).

**Remarks**

Ha effetto solo durante il salvataggio in TIFF. Il valore predefinito è Lzw.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```


Imposta il tipo di PhotometricInterpretation da applicare solo quando si salvano le pagine nel formato `Tiff`.

**Remarks**

Ha effetto solo durante il salvataggio in TIFF. Il valore predefinito è -1, indica che non viene applicata alcuna PhotometricInterpretation.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


Indica se lo sfondo dell'immagine generata deve essere trasparente.

**Remarks**

Il valore predefinito è false. Ciò significa che lo sfondo delle immagini generate è bianco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```


Imposta la risoluzione verticale per le immagini generate, in punti per pollice.

**Remarks**

Il valore predefinito è 96. Impostare  e  influisce sulla larghezza e altezza dell'immagine di output in pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


Imposta la callback di avviso.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

