---
title: PdfSaveOptions
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta le opzioni per il salvataggio del file pdf.
type: docs
weight: 4500
url: /it/net/aspose.cells/pdfsaveoptions/
---
## PdfSaveOptions class

Rappresenta le opzioni per il salvataggio del file pdf.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions#constructor)() | Crea le opzioni per il salvataggio del file pdf. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/pdfsaveoptions/allcolumnsinonepagepersheet) { get; set; } | Se AllColumnsInOnePagePerSheet è true , tutto il contenuto delle colonne di un foglio verrà restituito a una sola pagina nel risultato. La larghezza del formato carta di pagesetup verrà ignorata e le altre impostazioni di pagesetup avranno ancora effetto. |
| [Bookmark](../../aspose.cells/pdfsaveoptions/bookmark) { get; set; } | Ottiene e imposta il[`PdfBookmarkEntry`](../../aspose.cells.rendering/pdfbookmarkentry) oggetto. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | La cartella dei file nella cache viene utilizzata per memorizzare dati di grandi dimensioni. |
| [CalculateFormula](../../aspose.cells/pdfsaveoptions/calculateformula) { get; set; } | Indica se calcolare le formule prima di salvare il file pdf. |
| [CheckFontCompatibility](../../aspose.cells/pdfsaveoptions/checkfontcompatibility) { get; set; } | Indica se controllare la compatibilità dei font per ogni carattere del testo. |
| [CheckWorkbookDefaultFont](../../aspose.cells/pdfsaveoptions/checkworkbookdefaultfont) { get; set; } | Quando i caratteri in Excel sono Unicode e non possono essere impostati con il carattere corretto nello stile della cella, Possono apparire come blocchi in pdf, immagine. Impostalo su true per provare a utilizzare il carattere predefinito della cartella di lavoro per mostrare prima questi caratteri. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Rendi vuota la cartella di lavoro dopo aver salvato il file. |
| [Compliance](../../aspose.cells/pdfsaveoptions/compliance) { get; set; } | La cartella di lavoro viene convertita in pdf in base a PdfCompliance in questa proprietà. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [CreatedTime](../../aspose.cells/pdfsaveoptions/createdtime) { get; set; } | Ottiene e imposta l'ora di generazione del documento pdf. |
| [CustomPropertiesExport](../../aspose.cells/pdfsaveoptions/custompropertiesexport) { get; set; } | Ottiene o imposta un valore che determina il percorso[`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection) vengono esportati in file PDF. Il valore predefinito è Nessuno. |
| [DefaultEditLanguage](../../aspose.cells/pdfsaveoptions/defaulteditlanguage) { get; set; } | Ottiene o imposta la lingua di modifica predefinita. |
| [DefaultFont](../../aspose.cells/pdfsaveoptions/defaultfont) { get; set; } | Quando i caratteri in Excel sono Unicode e non possono essere impostati con il font corretto nello stile della cella, Possono apparire come blocchi in pdf,image. Impostare il DefaultFont come MingLiu o MS Gothic per mostrare questi caratteri. Se questa proprietà è non impostato, Aspose.Cells utilizzerà il carattere predefinito del sistema per mostrare questi caratteri unicode. |
| [DisplayDocTitle](../../aspose.cells/pdfsaveoptions/displaydoctitle) { get; set; } | Indica se la barra del titolo della finestra deve visualizzare il titolo del documento. |
| [DrawObjectEventHandler](../../aspose.cells/pdfsaveoptions/drawobjecteventhandler) { get; set; } | Implementa questa interfaccia per ottenere DrawObject e Bound durante il rendering. |
| [EmbedStandardWindowsFonts](../../aspose.cells/pdfsaveoptions/embedstandardwindowsfonts) { get; set; } | True per incorporare i caratteri di tipo true. Influisce solo sui caratteri ASCII 32-127. I caratteri per codici carattere maggiori di 127 sono sempre incorporati. I caratteri sono sempre incorporati per PDF/A-1a, PDF/A-1b standard. L'impostazione predefinita è true. |
| [EmfRenderSetting](../../aspose.cells/pdfsaveoptions/emfrendersetting) { get; set; } | Impostazione per il rendering del metafile Emf. |
| [ExportDocumentStructure](../../aspose.cells/pdfsaveoptions/exportdocumentstructure) { get; set; } | Indica se esportare la struttura del documento. |
| [FontEncoding](../../aspose.cells/pdfsaveoptions/fontencoding) { get; set; } | Ottiene o imposta la codifica dei caratteri incorporata in pdf. |
| [GridlineType](../../aspose.cells/pdfsaveoptions/gridlinetype) { get; set; } | Ottiene o imposta il tipo di griglia. |
| [IgnoreError](../../aspose.cells/pdfsaveoptions/ignoreerror) { get; set; } | Indica se è necessario nascondere l'errore durante il rendering. L'errore può essere un errore di forma, immagine, rendering del grafico, ecc. |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/pdfsaveoptions/isfontsubstitutionchargranularity) { get; set; } | Indica se sostituire il font del carattere solo quando il font della cella non è compatibile con esso. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Indica se unire le aree di formattazione condizionale e validazione prima di salvare il file. |
| [OnePagePerSheet](../../aspose.cells/pdfsaveoptions/onepagepersheet) { get; set; } | Se OnePagePerSheet è true , tutto il contenuto di un foglio verrà restituito a una sola pagina nel risultato. Il formato carta di pagesetup non sarà valido e le altre impostazioni di pagesetup avranno ancora effetto. |
| [OptimizationType](../../aspose.cells/pdfsaveoptions/optimizationtype) { get; set; } | Ottiene e imposta il tipo di ottimizzazione pdf. |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/pdfsaveoptions/outputblankpagewhennothingtoprint) { get; set; } | Indica se stampare una pagina vuota quando non c'è nulla da stampare. |
| [PageCount](../../aspose.cells/pdfsaveoptions/pagecount) { get; set; } | Ottiene o imposta il numero di pagine da salvare. |
| [PageIndex](../../aspose.cells/pdfsaveoptions/pageindex) { get; set; } | Ottiene o imposta l'indice in base 0 della prima pagina da salvare. |
| [PageSavingCallback](../../aspose.cells/pdfsaveoptions/pagesavingcallback) { get; set; } | Controlla/Indica l'avanzamento del processo di salvataggio della pagina. |
| [PdfCompression](../../aspose.cells/pdfsaveoptions/pdfcompression) { get; set; } | Indica l'algoritmo di compressione |
| [PrintingPageType](../../aspose.cells/pdfsaveoptions/printingpagetype) { get; set; } | Indica quali pagine non verranno stampate. |
| [Producer](../../aspose.cells/pdfsaveoptions/producer) { get; set; } | Ottiene e imposta il produttore del documento pdf generato. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Indica se aggiornare i dati della cache del grafico |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Ottiene il formato del file di salvataggio. |
| [SecurityOptions](../../aspose.cells/pdfsaveoptions/securityoptions) { get; set; } | Imposta queste opzioni, quando è necessaria la sicurezza nel risultato di xls2pdf. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. |
| [TextCrossType](../../aspose.cells/pdfsaveoptions/textcrosstype) { get; set; } | Ottiene o imposta la visualizzazione del tipo di testo quando la larghezza del testo è maggiore della larghezza della cella. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Indica se aggiornare l'impostazione Smart Art. Il valore predefinito è false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Ottiene o imposta la richiamata di avviso. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetImageResample](../../aspose.cells/pdfsaveoptions/setimageresample)(int, int) | Imposta i PPI (pixel per pollice) desiderati per ricampionare le immagini e la qualità jpeg. Tutte le immagini verranno convertite in JPEG con l'impostazione di qualità specificata, e le immagini che sono maggiori del PPI specificato (pixel per pollice) verranno ricampionate. |

### Guarda anche

* class [SaveOptions](../saveoptions)
* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
