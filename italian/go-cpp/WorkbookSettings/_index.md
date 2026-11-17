---
title: "Classe WorkbookSettings"
linktitle: "WorkbookSettings"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe WorkbookSettings. Incapsula l'oggetto che rappresenta le impostazioni della cartella di lavoro in Go."
type: docs
weight: 200
url: /it/go-cpp/workbooksettings/
---

## WorkbookSettings class

Rappresenta tutte le impostazioni della cartella di lavoro.

```go

type WorkbookSettings struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [Dispose](./dispose/) | Rilascia le risorse. |
| [GetThemeFont](./getthemefont/) | Ottiene il nome del carattere predefinito del tema. |
| [GetAuthor](./getauthor/) | Ottiene e imposta l'autore del file. |
| [SetAuthor](./setauthor/) | Ottiene e imposta l'autore del file. |
| [GetCheckCustomNumberFormat](./getcheckcustomnumberformat/) | Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom. |
| [SetCheckCustomNumberFormat](./setcheckcustomnumberformat/) | Indica se verificare il formato numerico personalizzato quando si imposta Style.Custom. |
| [GetEnableMacros](./getenablemacros/) | Abilita macro; |
| [SetEnableMacros](./setenablemacros/) | Abilita macro; |
| [GetDate1904](./getdate1904/) | Ottiene o imposta un valore che indica se la cartella di lavoro utilizza il sistema di data 1904. |
| [SetDate1904](./setdate1904/) | Ottiene o imposta un valore che indica se la cartella di lavoro utilizza il sistema di data 1904. |
| [GetProtectionType](./getprotectiontype/) | Ottiene il tipo di protezione della cartella di lavoro. |
| [GetDisplayDrawingObjects](./getdisplaydrawingobjects/) | Indica se e come mostrare gli oggetti nella cartella di lavoro. |
| [SetDisplayDrawingObjects](./setdisplaydrawingobjects/) | Indica se e come mostrare gli oggetti nella cartella di lavoro. |
| [GetSheetTabBarWidth](./getsheettabbarwidth/) | Larghezza della barra delle schede del foglio di lavoro (in 1/1000 della larghezza della finestra). |
| [SetSheetTabBarWidth](./setsheettabbarwidth/) | Larghezza della barra delle schede del foglio di lavoro (in 1/1000 della larghezza della finestra). |
| [GetShowTabs](./getshowtabs/) | Ottiene o imposta un valore che indica se le schede della cartella di lavoro sono visualizzate. |
| [SetShowTabs](./setshowtabs/) | Ottiene o imposta un valore che indica se le schede della cartella di lavoro sono visualizzate. |
| [GetFirstVisibleTab](./getfirstvisibletab/) | Ottiene o imposta la prima scheda del foglio di lavoro visibile. |
| [SetFirstVisibleTab](./setfirstvisibletab/) | Ottiene o imposta la prima scheda del foglio di lavoro visibile. |
| [IsHScrollBarVisible](./ishscrollbarvisible/) | Ottiene o imposta un valore che indica se il foglio elettronico generato conterrà una barra di scorrimento orizzontale. |
| [SetIsHScrollBarVisible](./setishscrollbarvisible/) | Ottiene o imposta un valore che indica se il foglio elettronico generato conterrà una barra di scorrimento orizzontale. |
| [IsVScrollBarVisible](./isvscrollbarvisible/) | Ottiene o imposta un valore che indica se il foglio elettronico generato conterrà una barra di scorrimento verticale. |
| [SetIsVScrollBarVisible](./setisvscrollbarvisible/) | Ottiene o imposta un valore che indica se il foglio elettronico generato conterrà una barra di scorrimento verticale. |
| [GetShared](./getshared/) | Ottiene o imposta un valore che indica se la cartella di lavoro è condivisa. |
| [SetShared](./setshared/) | Ottiene o imposta un valore che indica se la cartella di lavoro è condivisa. |
| [GetLanguageCode](./getlanguagecode/) | Ottiene o imposta la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file. |
| [SetLanguageCode](./setlanguagecode/) | Ottiene o imposta la lingua dell'interfaccia utente della versione della Cartella di lavoro basata sul CountryCode con cui è stato salvato il file. |
| [GetRegion](./getregion/) | Ottiene o imposta le impostazioni regionali per la cartella di lavoro. |
| [SetRegion](./setregion/) | Ottiene o imposta le impostazioni regionali per la cartella di lavoro. |
| [GetGlobalizationSettings](./getglobalizationsettings/) | Ottiene e imposta le impostazioni di globalizzazione. |
| [SetGlobalizationSettings](./setglobalizationsettings/) | Ottiene e imposta le impostazioni di globalizzazione. |
| [GetNumberDecimalSeparator](./getnumberdecimalseparator/) | Ottiene o imposta il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della regione corrente. |
| [SetNumberDecimalSeparator](./setnumberdecimalseparator/) | Ottiene o imposta il separatore decimale per la formattazione/analisi dei valori numerici. Il valore predefinito è il separatore decimale della regione corrente. |
| [GetNumberGroupSeparator](./getnumbergroupseparator/) | Ottiene o imposta il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. Il valore predefinito è il separatore di gruppo della regione corrente. |
| [SetNumberGroupSeparator](./setnumbergroupseparator/) | Ottiene o imposta il carattere che separa i gruppi di cifre a sinistra del decimale nei valori numerici. Il valore predefinito è il separatore di gruppo della regione corrente. |
| [GetPassword](./getpassword/) | Rappresenta la password di crittografia del file della cartella di lavoro. |
| [SetPassword](./setpassword/) | Rappresenta la password di crittografia del file della cartella di lavoro. |
| [GetWriteProtection](./getwriteprotection/) | Fornisce l'accesso alle opzioni di protezione in scrittura della cartella di lavoro. |
| [IsEncrypted](./isencrypted/) | Ottiene un valore che indica se è richiesta una password per aprire questo workbook. |
| [IsProtected](./isprotected/) | Ottiene un valore che indica se la struttura o la finestra del Workbook è protetta. |
| [IsDefaultEncrypted](./isdefaultencrypted/) | Indica se crittografare il workbook con password predefinita se Structure e Windows del workbook sono bloccati. |
| [SetIsDefaultEncrypted](./setisdefaultencrypted/) | Indica se crittografare il workbook con password predefinita se Structure e Windows del workbook sono bloccati. |
| [IsMinimized](./isminimized/) | Rappresenta se il foglio di calcolo generato sarà aperto Minimized. |
| [SetIsMinimized](./setisminimized/) | Rappresenta se il foglio di calcolo generato sarà aperto Minimized. |
| [IsHidden](./ishidden/) | Indica se questo workbook è nascosto. |
| [SetIsHidden](./setishidden/) | Indica se questo workbook è nascosto. |
| [GetAutoCompressPictures](./getautocompresspictures/) | Specifica un valore booleano che indica se l'applicazione comprime automaticamente le immagini nel workbook. |
| [SetAutoCompressPictures](./setautocompresspictures/) | Specifica un valore booleano che indica se l'applicazione comprime automaticamente le immagini nel workbook. |
| [GetRemovePersonalInformation](./getremovepersonalinformation/) | True se le informazioni personali possono essere rimosse dal workbook specificato. |
| [SetRemovePersonalInformation](./setremovepersonalinformation/) | True se le informazioni personali possono essere rimosse dal workbook specificato. |
| [GetShapeDisplayType](./getshapedisplaytype/) | Ottiene e imposta come l'applicazione visualizza le forme in questo workbook |
| [SetShapeDisplayType](./setshapedisplaytype/) | Ottiene e imposta come l'applicazione visualizza le forme in questo workbook |
| [GetHidePivotFieldList](./gethidepivotfieldlist/) | Ottiene e imposta se nascondere l'elenco dei campi per la PivotTable. |
| [SetHidePivotFieldList](./sethidepivotfieldlist/) | Ottiene e imposta se nascondere l'elenco dei campi per la PivotTable. |
| [GetMaxUniqueItemsPerField](./getmaxuniqueitemsperfield/) | Ottiene e imposta la limitazione di elementi unici per campo |
| [SetMaxUniqueItemsPerField](./setmaxuniqueitemsperfield/) | Ottiene e imposta la limitazione di elementi unici per campo |
| [GetUpdateLinksType](./getupdatelinkstype/) | Ottiene e imposta come aggiornare i collegamenti esterni quando il workbook è aperto. |
| [SetUpdateLinksType](./setupdatelinkstype/) | Ottiene e imposta come aggiornare i collegamenti esterni quando il workbook è aperto. |
| [SetPageOrientationType](./setpageorientationtype/) | Imposta il tipo di orientamento di stampa per l'intero workbook. |
| [GetMaxRow](./getmaxrow/) | Ottiene l'indice massimo di riga, basato su zero. |
| [GetMaxColumn](./getmaxcolumn/) | Ottiene l'indice massimo di colonna, basato su zero. |
| [GetSmartTagOptions](./getsmarttagoptions/) | Ottiene le opzioni dello smart tag. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Ottiene le impostazioni per i valori predefiniti delle proprietà relative allo stile per questo workbook. |
| [GetWindowLeft](./getwindowleft/) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra, in unità di punto. |
| [SetWindowLeft](./setwindowleft/) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra, in unità di punto. |
| [GetWindowLeftInch](./getwindowleftinch/) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di pollice. |
| [SetWindowLeftInch](./setwindowleftinch/) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di pollice. |
| [GetWindowLeftCM](./getwindowleftcm/) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di centimetro. |
| [SetWindowLeftCM](./setwindowleftcm/) | La distanza dal bordo sinistro dell'area client al bordo sinistro della finestra. In unità di centimetro. |
| [GetWindowTop](./getwindowtop/) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di punto. |
| [SetWindowTop](./setwindowtop/) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di punto. |
| [GetWindowTopInch](./getwindowtopinch/) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di pollice. |
| [SetWindowTopInch](./setwindowtopinch/) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di pollice. |
| [GetWindowTopCM](./getwindowtopcm/) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di centimetro. |
| [SetWindowTopCM](./setwindowtopcm/) | La distanza dal bordo superiore dell'area client al bordo superiore della finestra, in unità di centimetro. |
| [GetWindowWidth](./getwindowwidth/) | La larghezza della finestra, in unità di punto. |
| [SetWindowWidth](./setwindowwidth/) | La larghezza della finestra, in unità di punto. |
| [GetWindowWidthInch](./getwindowwidthinch/) | La larghezza della finestra, in unità di pollice. |
| [SetWindowWidthInch](./setwindowwidthinch/) | La larghezza della finestra, in unità di pollice. |
| [GetWindowWidthCM](./getwindowwidthcm/) | La larghezza della finestra, in unità di centimetro. |
| [SetWindowWidthCM](./setwindowwidthcm/) | La larghezza della finestra, in unità di centimetro. |
| [GetWindowHeight](./getwindowheight/) | L'altezza della finestra, in unità di punto. |
| [SetWindowHeight](./setwindowheight/) | L'altezza della finestra, in unità di punto. |
| [GetWindowHeightInch](./getwindowheightinch/) | L'altezza della finestra, in unità di pollice. |
| [SetWindowHeightInch](./setwindowheightinch/) | L'altezza della finestra, in unità di pollice. |
| [GetWindowHeightCM](./getwindowheightcm/) | L'altezza della finestra, in unità di centimetro. |
| [SetWindowHeightCM](./setwindowheightcm/) | L'altezza della finestra, in unità di centimetro. |
| [GetUpdateAdjacentCellsBorder](./getupdateadjacentcellsborder/) | Indica se aggiornare il bordo delle celle adiacenti. |
| [SetUpdateAdjacentCellsBorder](./setupdateadjacentcellsborder/) | Indica se aggiornare il bordo delle celle adiacenti. |
| [GetSignificantDigitsType](./getsignificantdigitstype/) | Ottiene e imposta il tipo di cifre significative per l'emissione di numericvalues in questa cartella di lavoro. Il valore predefinito è CellsHelper.SignificantDigitsType. |
| [SetSignificantDigitsType](./setsignificantdigitstype/) | Ottiene e imposta il tipo di cifre significative per l'emissione di numericvalues in questa cartella di lavoro. Il valore predefinito è CellsHelper.SignificantDigitsType. |
| [GetCheckCompatibility](./getcheckcompatibility/) | Indica se verificare la compatibilità con versioni precedenti durante il salvataggio della cartella di lavoro. |
| [SetCheckCompatibility](./setcheckcompatibility/) | Indica se verificare la compatibilità con versioni precedenti durante il salvataggio della cartella di lavoro. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true, si otterrà un'Exception. Se questa proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è non valido per il formato file Excel, non dovresti salvare la cartella di lavoro come formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true, si otterrà un'Exception. Se questa proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è non valido per il formato file Excel, non dovresti salvare la cartella di lavoro come formato Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato. |
| [GetAutoRecover](./getautorecover/) | Indica se il file è contrassegnato per il recupero automatico. |
| [SetAutoRecover](./setautorecover/) | Indica se il file è contrassegnato per il recupero automatico. |
| [GetCrashSave](./getcrashsave/) | Indica se l'applicazione ha salvato l'ultimo file della cartella di lavoro dopo un arresto anomalo. |
| [SetCrashSave](./setcrashsave/) | Indica se l'applicazione ha salvato l'ultimo file della cartella di lavoro dopo un arresto anomalo. |
| [GetDataExtractLoad](./getdataextractload/) | Indica se l'applicazione ha aperto per ultimo la cartella di lavoro per il recupero dati. |
| [SetDataExtractLoad](./setdataextractload/) | Indica se l'applicazione ha aperto per ultimo la cartella di lavoro per il recupero dati. |
| [GetRepairLoad](./getrepairload/) | Indica se l'applicazione ha aperto per ultimo la cartella di lavoro in modalità sicura o di riparazione. |
| [SetRepairLoad](./setrepairload/) | Indica se l'applicazione ha aperto per ultimo la cartella di lavoro in modalità sicura o di riparazione. |
| [GetBuildVersion](./getbuildversion/) | Specifica il rilascio pubblico incrementale dell'applicazione. |
| [SetBuildVersion](./setbuildversion/) | Specifica il rilascio pubblico incrementale dell'applicazione. |
| [GetMemorySetting](./getmemorysetting/) | Ottiene o imposta le opzioni di utilizzo della memoria. La nuova opzione sarà presa come opzione predefinita per i fogli di lavoro appena creati ma non avrà effetto sui fogli di lavoro esistenti. |
| [SetMemorySetting](./setmemorysetting/) | Ottiene o imposta le opzioni di utilizzo della memoria. La nuova opzione sarà presa come opzione predefinita per i fogli di lavoro appena creati ma non avrà effetto sui fogli di lavoro esistenti. |
| [GetPaperSize](./getpapersize/) | Ottiene e imposta la dimensione carta di stampa predefinita. |
| [SetPaperSize](./setpapersize/) | Ottiene e imposta la dimensione carta di stampa predefinita. |
| [GetMaxRowsOfSharedFormula](./getmaxrowsofsharedformula/) | Ottiene e imposta il numero massimo di righe della formula condivisa. |
| [SetMaxRowsOfSharedFormula](./setmaxrowsofsharedformula/) | Ottiene e imposta il numero massimo di righe della formula condivisa. |
| [GetCompliance](./getcompliance/) | Specifica la versione OOXML per il documento di output. Il valore predefinito è Ecma376_2006. |
| [SetCompliance](./setcompliance/) | Specifica la versione OOXML per il documento di output. Il valore predefinito è Ecma376_2006. |
| [GetQuotePrefixToStyle](./getquoteprefixtostyle/) | Indica se impostare la proprietà Style.QuotePrefix quando si inserisce il valore stringa (che inizia con un apice singolo) nella cella. |
| [SetQuotePrefixToStyle](./setquoteprefixtostyle/) | Indica se impostare la proprietà Style.QuotePrefix quando si inserisce il valore stringa (che inizia con un apice singolo) nella cella. |
| [GetFormulaSettings](./getformulasettings/) | Ottiene le impostazioni per le funzionalità correlate alle formule. |
| [GetPropertiesFollowChartPoint](./getpropertiesfollowchartpoint/) | Indica se le proprietà dei datapoint e le datalabels in tutti i grafici di questa cartella di lavoro seguono il loro riferimento. |
| [SetPropertiesFollowChartPoint](./setpropertiesfollowchartpoint/) | Indica se le proprietà dei datapoint e le datalabels in tutti i grafici di questa cartella di lavoro seguono il loro riferimento. |
| [GetDiscardImageEditData](./getdiscardimageeditdata/) | Indica se scartare i dati immagine editting. |
| [SetDiscardImageEditData](./setdiscardimageeditdata/) | Indica se scartare i dati immagine editting. |
| [GetDefaultImageResolution](./getdefaultimageresolution/) | Ottiene e imposta la risoluzione predefinita dell'immagine. |
| [SetDefaultImageResolution](./setdefaultimageresolution/) | Ottiene e imposta la risoluzione predefinita dell'immagine. |
| [GetWpsCompatibility](./getwpscompatibility/) | Indica se essere compatibile con WPS. |
| [SetWpsCompatibility](./setwpscompatibility/) | Indica se essere compatibile con WPS. |
