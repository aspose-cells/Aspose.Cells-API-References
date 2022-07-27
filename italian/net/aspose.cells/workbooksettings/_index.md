---
title: WorkbookSettings
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta tutte le impostazioni della cartella di lavoro.
type: docs
weight: 6500
url: /it/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

Rappresenta tutte le impostazioni della cartella di lavoro.

```csharp
public class WorkbookSettings : IDisposable
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | Ottiene e imposta l'autore del file. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | Specifica un valore booleano che indica che l'applicazione ha compresso automaticamente le immagini nella cartella di lavoro. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | Indica se il file è contrassegnato per il ripristino automatico. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | Specifica la versione pubblica incrementale dell'applicazione. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | Indica se verificare la compatibilità con le versioni precedenti durante il salvataggio della cartella di lavoro. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | Indica se controllare il formato numero personalizzato quando si imposta Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | Indica se controllare la restrizione del file excel quando l'utente modifica gli oggetti correlati alle celle. Ad esempio, excel non consente l'immissione di un valore di stringa più lungo di 32K. Quando si immette un valore più lungo di 32K, ad esempio da Cell.PutValue(string), se questo è true, otterrai un'eccezione. Se questa proprietà è falsa, accetteremo il valore della stringa di input come valore della cella in modo che later tu possa restituire il valore della stringa completo per altri formati di file come CSV. Tuttavia, se hai impostato un tale tipo di valore che non è valido per il formato di file excel, non dovresti salvare la cartella di lavoro come formato di file excel in un secondo momento. Altrimenti potrebbe esserci un errore imprevisto per il file excel generato. |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | Specifica la versione OOXML per il documento di output. Il valore predefinito è Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | indica se l'applicazione ha salvato il file della cartella di lavoro l'ultima volta dopo un arresto anomalo. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | Ottiene o imposta le informazioni sulle impostazioni cultura del sistema. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | indica se l'applicazione ha aperto per l'ultima volta la cartella di lavoro per il ripristino dei dati. |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | Ottiene o imposta un valore che rappresenta se la cartella di lavoro utilizza il sistema di data 1904. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | Indica se e come mostrare gli oggetti nella cartella di lavoro. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | Abilita macro; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | Ottiene o imposta la prima scheda del foglio di lavoro visibile. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | Ottiene le impostazioni per le funzioni relative alle formule. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | Ottiene e imposta le impostazioni di globalizzazione. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | Ottiene e imposta se nascondere l'elenco dei campi per la tabella pivot. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | Indica se crittografare la cartella di lavoro con password predefinita se la Struttura e le finestre della cartella di lavoro sono bloccate. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | Ottiene un valore che indica se è necessaria una password per aprire questa cartella di lavoro. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | Indica se questa cartella di lavoro è nascosta. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | Ottiene o imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento orizzontale. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | Indica se il foglio di calcolo generato verrà aperto Ridotto a icona. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | Ottiene un valore che indica se la struttura o la finestra della cartella di lavoro è protetta. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | Ottiene o imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento verticale. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione della cartella di lavoro in base a CountryCode che ha salvato il file. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | Ottiene l'indice di colonna massimo, in base zero. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | Ottiene l'indice di riga massimo, in base zero. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | Ottiene e imposta il numero massimo di righe della formula condivisa. |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | Ottiene o imposta le opzioni di utilizzo della memoria. La nuova opzione verrà presa come opzione predefinita per i fogli di lavoro appena creati, ma non avrà effetto per i fogli di lavoro esistenti. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | Ottiene o imposta il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della regione corrente. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | Ottiene o imposta il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. L'impostazione predefinita è il separatore di gruppo della regione corrente. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | Ottiene e imposta il formato carta di stampa predefinito. |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | Rappresenta la password di crittografia del file della cartella di lavoro. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | Ottiene il tipo di protezione della cartella di lavoro. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | Indica se l'impostazione[`QuotePrefix`](../style/quoteprefix) proprietà quando si immette il valore della stringa (che inizia con virgolette singole ) nella cella |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | Ottiene o imposta le impostazioni internazionali per la cartella di lavoro. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | True se le informazioni personali possono essere rimosse dalla cartella di lavoro specificata. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | Indica se l'applicazione ha aperto la cartella di lavoro l'ultima volta in modalità provvisoria o di ripristino. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | Ottiene e imposta il provider di flusso per la risorsa esterna, ad esempio il caricamento dei dati dell'immagine per l'immagine di tipo "LinkToFile". |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | Ottiene o imposta un valore che indica se la cartella di lavoro è condivisa. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | Larghezza della barra delle schede del foglio di lavoro (in 1/1000 della larghezza della finestra). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | Recupera o imposta un valore indipendentemente dalla visualizzazione delle schede Cartella di lavoro. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | Ottiene e imposta il numero di cifre significative. Il valore predefinito è[`SignificantDigits`](../cellshelper/significantdigits) . |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | Indica se aggiornare il bordo delle celle adiacenti. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | Ottiene e imposta la modalità di aggiornamento dei collegamenti esterni all'apertura della cartella di lavoro. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | Ottiene o imposta la richiamata di avviso. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | L'altezza della finestra, in unità di punti. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | L'altezza della finestra, in unità di centimetri. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | L'altezza della finestra, in unità di pollici. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra, in unità di punti. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di centimetri. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di pollici. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di punti. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di centimetri. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di pollici. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | La larghezza della finestra, in unità di punti. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | La larghezza della finestra, in unità di centimetri. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | La larghezza della finestra, in unità di pollici. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | Fornisce l'accesso alle opzioni di protezione dalla scrittura della cartella di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | Rilascia risorse. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | Ottiene il nome del carattere del tema predefinito. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | Imposta il tipo di orientamento di stampa per l'intera cartella di lavoro. |

### Esempi

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

//fai i tuoi affari

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'fai i tuoi affari
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
