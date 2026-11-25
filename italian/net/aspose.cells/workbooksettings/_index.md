---
title: "Classe WorkbookSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.WorkbookSettings. Rappresenta tutte le impostazioni della cartella di lavoro"
type: docs
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
| [Author](../../aspose.cells/workbooksettings/author/) { get; set; } | Ottiene e imposta l'autore del file. |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures/) { get; set; } | Specifica un valore booleano che indica che l'applicazione comprime automaticamente le immagini nella cartella di lavoro. |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover/) { get; set; } | Indica se il file è contrassegnato per il recupero automatico. |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion/) { get; set; } | Specifica la versione incrementale pubblica dell'applicazione. |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility/) { get; set; } | Indica se verificare la compatibilità con versioni precedenti durante il salvataggio della workbook. |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat/) { get; set; } | Indica se controllare il formato numerico personalizzato quando si imposta Style.Custom. |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true otterrai un'Exception. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato file excel, non dovresti salvare la workbook in formato excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file excel generato. |
| [Compliance](../../aspose.cells/workbooksettings/compliance/) { get; set; } | Specifica la versione OOXML per il documento di output. Il valore predefinito è Ecma376_2006. |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave/) { get; set; } | Indica se l'applicazione ha salvato l'ultimo file workbook dopo un arresto anomalo. |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo/) { get; set; } | Ottiene o imposta le informazioni sulla cultura di sistema. |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload/) { get; set; } | Indica se l'applicazione ha aperto per l'ultima volta la workbook per il recupero dati. |
| [Date1904](../../aspose.cells/workbooksettings/date1904/) { get; set; } | Ottiene o imposta un valore che indica se la workbook utilizza il sistema di data 1904. |
| [DefaultImageResolution](../../aspose.cells/workbooksettings/defaultimageresolution/) { get; set; } | Ottiene e imposta la risoluzione predefinita dell'immagine. |
| [DefaultStyleSettings](../../aspose.cells/workbooksettings/defaultstylesettings/) { get; } | Ottiene le impostazioni per i valori predefiniti delle proprietà relative allo stile per questa workbook. |
| [DiscardImageEditData](../../aspose.cells/workbooksettings/discardimageeditdata/) { get; set; } | Indica se scartare i dati di immagine in fase di modifica. |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects/) { get; set; } | Indica se e come mostrare gli oggetti nella workbook. |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros/) { get; set; } | Abilita le macro; |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab/) { get; set; } | Ottiene o imposta la prima scheda del foglio di lavoro visibile. |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings/) { get; } | Ottiene le impostazioni per le funzionalità relative alle formule. |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings/) { get; set; } | Ottiene e imposta le impostazioni di globalizzazione. |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist/) { get; set; } | Ottiene e imposta se nascondere l'elenco dei campi per la PivotTable. |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted/) { get; set; } | Indica se crittografare la workbook con password predefinita se Structure e Windows della workbook sono bloccati. |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted/) { get; } | Ottiene un valore che indica se è necessaria una password per aprire questa workbook. |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden/) { get; set; } | Indica se questa workbook è nascosta. |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible/) { get; set; } | Ottiene o imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento orizzontale. |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized/) { get; set; } | Rappresenta se il foglio di calcolo generato sarà aperto ridotto a icona. |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected/) { get; } | Ottiene un valore che indica se la struttura o la finestra del Workbook è protetta. |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible/) { get; set; } | Ottiene o imposta un valore che indica se il foglio di calcolo generato conterrà una barra di scorrimento verticale. |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode/) { get; set; } | Ottiene o imposta la lingua dell'interfaccia utente della versione del Workbook basata sul CountryCode che ha salvato il file. |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn/) { get; } | Ottiene l'indice massimo della colonna, a base zero. |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow/) { get; } | Ottiene l'indice massimo della riga, a base zero. |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula/) { get; set; } | Ottiene e imposta il numero massimo di righe della formula condivisa. |
| [MaxUniqueItemsPerField](../../aspose.cells/workbooksettings/maxuniqueitemsperfield/) { get; set; } | Ottiene e imposta il limite di elementi unici per campo |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting/) { get; set; } | Ottiene o imposta le opzioni di utilizzo della memoria. La nuova opzione sarà presa come opzione predefinita per i fogli di lavoro appena creati, ma non avrà effetto sui fogli di lavoro esistenti. |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator/) { get; set; } | Ottiene o imposta il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della Regione corrente. |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator/) { get; set; } | Ottiene o imposta il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. Il valore predefinito è il separatore di gruppo della Regione corrente. |
| [PaperSize](../../aspose.cells/workbooksettings/papersize/) { get; set; } | Ottiene e imposta la dimensione predefinita della carta di stampa. |
| [Password](../../aspose.cells/workbooksettings/password/) { get; set; } | Rappresenta la password di crittografia del file Workbook. |
| [PropertiesFollowChartPoint](../../aspose.cells/workbooksettings/propertiesfollowchartpoint/) { get; set; } | Indica se le proprietà dei punti dati e le etichette dei dati in tutti i grafici di questo workbook seguono il loro riferimento. |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype/) { get; } | Ottiene il tipo di protezione del workbook. |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle/) { get; set; } | Indica se l'impostazione della proprietà [`QuotePrefix`](../style/quoteprefix/) quando si inserisce il valore stringa (che inizia con un apice singolo) nella cella |
| [Region](../../aspose.cells/workbooksettings/region/) { get; set; } | Ottiene o imposta le impostazioni regionali per il workbook. |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation/) { get; set; } | Vero se le informazioni personali possono essere rimosse dal workbook specificato. |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload/) { get; set; } | Indica se l'applicazione ha aperto l'ultimo workbook in modalità sicura o di riparazione. |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider/) { get; set; } | Ottiene e imposta il provider di stream per risorse esterne, come il caricamento dei dati immagine per un'immagine di tipo "LinkToFile". |
| [ShapeDisplayType](../../aspose.cells/workbooksettings/shapedisplaytype/) { get; set; } | Ottiene e imposta come l'applicazione visualizza le forme in questo workbook |
| [Shared](../../aspose.cells/workbooksettings/shared/) { get; set; } | Ottiene o imposta un valore che indica se il Workbook è condiviso. |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth/) { get; set; } | Larghezza della barra delle schede del foglio di lavoro (in 1/1000 della larghezza della finestra). |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs/) { get; set; } | Ottiene o imposta un valore che indica se le schede del Workbook sono visualizzate. |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits/) { get; set; } | (**Obsoleto.**) Ottiene e imposta il numero di cifre significative. Il valore predefinito è [`SignificantDigits`](../cellshelper/significantdigits/). |
| [SignificantDigitsType](../../aspose.cells/workbooksettings/significantdigitstype/) { get; set; } | Ottiene e imposta il tipo di cifre significative per l'emissione di valori numerici in questo workbook. Il valore predefinito è [`SignificantDigitsType`](../cellshelper/significantdigitstype/). |
| [SmartTagOptions](../../aspose.cells/workbooksettings/smarttagoptions/) { get; } | Ottiene le opzioni del tag intelligente. |
| [StreamProvider](../../aspose.cells/workbooksettings/streamprovider/) { get; set; } | (**Obsolete.**) Ottiene e imposta il provider di flusso per la risorsa esterna. |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder/) { get; set; } | Indica se aggiornare il bordo delle celle adiacenti. |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype/) { get; set; } | Ottiene e imposta come aggiornare i collegamenti esterni quando la cartella di lavoro viene aperta. |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback/) { get; set; } | Ottiene o imposta il callback di avviso. |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight/) { get; set; } | L'altezza della finestra, in unità di punto. |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm/) { get; set; } | L'altezza della finestra, in unità di centimetro. |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch/) { get; set; } | L'altezza della finestra, in unità di pollice. |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft/) { get; set; } | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra, in unità di punto. |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm/) { get; set; } | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di centimetro. |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch/) { get; set; } | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di pollice. |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop/) { get; set; } | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di punto. |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm/) { get; set; } | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di centimetro. |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch/) { get; set; } | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di pollice. |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth/) { get; set; } | La larghezza della finestra, in unità di punto. |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm/) { get; set; } | La larghezza della finestra, in unità di centimetro. |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch/) { get; set; } | La larghezza della finestra, in unità di pollice. |
| [WpsCompatibility](../../aspose.cells/workbooksettings/wpscompatibility/) { get; set; } | Indica se essere compatibile con WPS. |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection/) { get; } | Fornisce l'accesso alle opzioni di protezione in scrittura della cartella di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose/)() | Rilascia le risorse. |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont/)(FontSchemeType) | Ottiene il nome del carattere predefinito del tema. |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype/)(PageOrientationType) | Imposta il tipo di orientamento di stampa per l'intera cartella di lavoro. |

### Esempi

```csharp
using Aspose.Cells;
using System;
using System.Globalization;

public class WorkbookSettingsDemo
{
    public static void RunDemo()
    {
        // Crea un nuovo workbook
        Workbook workbook = new Workbook();
        Worksheet sheet = workbook.Worksheets[0];

        // Aggiungi alcuni dati di esempio
        sheet.Cells["A1"].PutValue("Sample Data");
        sheet.Cells["A2"].PutValue(123);
        sheet.Cells["A3"].PutValue(DateTime.Now);

        // Accedi a WorkbookSettings
        WorkbookSettings settings = workbook.Settings;

        // Imposta varie impostazioni
        settings.Author = "John Doe";
        settings.CheckCustomNumberFormat = true;
        settings.EnableMacros = false;
        settings.Date1904 = false;
        settings.DisplayDrawingObjects = DisplayDrawingObjects.DisplayShapes;
        settings.SheetTabBarWidth = 1000;
        settings.ShowTabs = true;
        settings.FirstVisibleTab = 0;
        settings.IsHScrollBarVisible = true;
        settings.IsVScrollBarVisible = true;
        settings.Shared = false;
        settings.LanguageCode = CountryCode.USA;
        settings.Region = CountryCode.USA;
        settings.CultureInfo = new CultureInfo("en-US");
        settings.GlobalizationSettings = new GlobalizationSettings();
        settings.NumberDecimalSeparator = '.';
        settings.NumberGroupSeparator = ',';
        settings.Password = "password123";
        settings.IsDefaultEncrypted = false;
        settings.IsMinimized = false;
        settings.IsHidden = false;
        settings.AutoCompressPictures = true;
        settings.RemovePersonalInformation = false;
        settings.HidePivotFieldList = false;
        settings.UpdateLinksType = UpdateLinksType.UserSet;
        settings.WindowLeft = 0;
        settings.WindowLeftInch = 0;
        settings.WindowLeftCM = 0;
        settings.WindowTop = 0;
        settings.WindowTopInch = 0;
        settings.WindowTopCM = 0;
        settings.WindowWidth = 800;
        settings.WindowWidthInch = 8;
        settings.WindowWidthCM = 20.32;
        settings.WindowHeight = 600;
        settings.WindowHeightInch = 6;
        settings.WindowHeightCM = 15.24;
        settings.UpdateAdjacentCellsBorder = true;
        settings.SignificantDigits = 15;
        settings.CheckCompatibility = true;
        settings.CheckExcelRestriction = true;
        settings.AutoRecover = true;
        settings.CrashSave = false;
        settings.DataExtractLoad = false;
        settings.RepairLoad = false;
        settings.BuildVersion = "1.0.0";
        settings.MemorySetting = MemorySetting.Normal;
        settings.PaperSize = PaperSizeType.PaperA4;
        settings.WarningCallback = null;
        settings.MaxRowsOfSharedFormula = 1048576;
        settings.Compliance = OoxmlCompliance.Ecma376_2006;
        settings.QuotePrefixToStyle = false;

        // Salva la cartella di lavoro
        workbook.Save("WorkbookSettingsDemo.xlsx");
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


