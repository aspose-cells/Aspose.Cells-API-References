---
title: "Classe Workbook"
linktitle: "Workbook"
second_title: "Riferimento API C++ di Aspose.Cells per Go"
description: "Classe Workbook. Incapsula l'oggetto che rappresenta il workbook in Go."
type: docs
weight: 200
url: /it/go-cpp/workbook/
---

## Workbook class

Rappresenta un oggetto radice per creare un foglio di calcolo Excel.

```go

type Workbook struct  {
	ptr unsafe.Pointer
}

```
## Costruttori

| Metodo | Descrizione |
| --- | --- |
| [NewWorkbook](./newworkbook/) | Inizializza una nuova istanza della classe Workbook. |
| [NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | Inizializza una nuova istanza della classe Workbook. |
| [NewWorkbook_LoadOptions](./newworkbook_loadoptions/) | Inizializza una nuova istanza vuota della classe Workbook con opzioni |
| [NewWorkbook_String](./newworkbook_string/) | Inizializza una nuova istanza della classe Workbook e apre un file. |
| [NewWorkbook_Stream](./newworkbook_stream/) | Inizializza una nuova istanza della classe Workbook e apre uno stream. |
| [NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | Inizializza una nuova istanza della classe Workbook e apre un file. |
| [NewWorkbook_Stream_LoadOptions](./newworkbook_stream_loadoptions/) | Inizializza una nuova istanza della classe Workbook e apre lo stream. |

## Metodi

| Metodo | Descrizione |
| --- | --- |
| [IsNull](./isnull/) | Verifica se l'oggetto di implementazione è nullptr. |
| [GetSettings](./getsettings/) | Rappresenta le impostazioni del workbook. |
| [ParseFormulas](./parseformulas/) | Analizza tutte le formule che non sono state analizzate quando sono state caricate dal file modello o impostate in una cella. |
| [StartAccessCache](./startaccesscache/) | Avvia la sessione che utilizza cache per accedere ai dati. |
| [CloseAccessCache](./closeaccesscache/) | Chiude la sessione che utilizza cache per accedere ai dati. |
| [Save_String_SaveFormat](./save_string_saveformat/) | Salva la cartella di lavoro su disco. |
| [Save_String](./save_string/) | Salva la cartella di lavoro su disco. |
| [Save_String_SaveOptions](./save_string_saveoptions/) | Salva la cartella di lavoro su disco. |
| [Save_SaveFormat](./save_saveformat/) | Salva la cartella di lavoro sullo stream. |
| [Save_SaveOptions](./save_saveoptions/) | Salva la cartella di lavoro sullo stream. |
| [SaveToStream](./savetostream/) | Salva il file Excel in un oggetto MemoryStream come file Excel97-2003 xls e lo restituisce. |
| [GetWorksheets](./getworksheets/) | Ottiene la collezione WorksheetCollection nel foglio di calcolo. |
| [IsLicensed](./islicensed/) | Indica se la licenza è impostata. |
| [RemoveUnusedStyles](./removeunusedstyles/) | Rimuove tutti gli stili non utilizzati. |
| [CreateStyle](./createstyle/) | Crea un nuovo stile. |
| [CreateStyle_Bool](./createstyle_bool/) | Crea un nuovo stile. |
| [CreateBuiltinStyle](./createbuiltinstyle/) | Crea uno stile predefinito del tipo specificato. |
| [CreateCellsColor](./createcellscolor/) | Crea un oggetto CellsColor. |
| [Replace_String_String](./replace_string_string/) | Sostituisce il valore di una cella con una nuova stringa. |
| [Replace_String_Int](./replace_string_int/) | Sostituisce il valore di una cella con un nuovo intero. |
| [Replace_String_Double](./replace_string_double/) | Sostituisce il valore di una cella con un nuovo double. |
| [Replace_String_stringArray_Bool](./replace_string_stringarray_bool/) | Sostituisce il valore di una cella con un nuovo array di stringhe. |
| [Replace_String_int32Array_Bool](./replace_string_int32array_bool/) | Sostituisce i valori delle celle con un array di interi. |
| [Replace_String_float64Array_Bool](./replace_string_float64array_bool/) | Sostituisce i valori delle celle con un array di double. |
| [Replace_Bool_Object](./replace_bool_object/) | Sostituisce i valori delle celle con nuovi dati. |
| [Replace_Int_Object](./replace_int_object/) | Sostituisce i valori delle celle con nuovi dati. |
| [Replace_String_String_ReplaceOptions](./replace_string_string_replaceoptions/) | Sostituisce il valore di una cella con una nuova stringa. |
| [Copy_Workbook_CopyOptions](./copy_workbook_copyoptions/) | Copia un altro oggetto Workbook. |
| [Copy_Workbook](./copy_workbook/) | Copia i dati da un oggetto Workbook di origine. |
| [Combine](./combine/) | Combina un altro oggetto Workbook. |
| [GetColors](./getcolors/) | Restituisce i colori nella palette per il foglio di calcolo. |
| [GetStyleInPool](./getstyleinpool/) | Ottiene lo stile nel pool di stili. Tutti gli stili nella cartella di lavoro saranno raccolti in un pool. Nelle celle è presente solo un semplice indice di riferimento. |
| [GetCountOfStylesInPool](./getcountofstylesinpool/) | Ottiene il numero degli stili nel pool di stili. |
| [GetFonts](./getfonts/) | Ottiene tutti i font nel pool di stili. |
| [GetNamedStyle](./getnamedstyle/) | Ottiene lo stile denominato nel pool di stili. |
| [MergeNamedStyles](./mergenamedstyles/) | Unisce gli stili denominati dall'altro file Excel. |
| [ChangePalette](./changepalette/) | Modifica la tavolozza per il foglio di calcolo nell'indice specificato. |
| [IsColorInPalette](./iscolorinpalette/) | Verifica se un colore è nella tavolozza per il foglio di calcolo. |
| [CalculateFormula](./calculateformula/) | Calcola il risultato delle formule. |
| [CalculateFormula_Bool](./calculateformula_bool/) | Calcola il risultato delle formule. |
| [CalculateFormula_CalculationOptions](./calculateformula_calculationoptions/) | Calcolo delle formule in questa cartella di lavoro. |
| [RefreshDynamicArrayFormulas_Bool](./refreshdynamicarrayformulas_bool/) | Aggiorna le formule di array dinamici (espansione in un nuovo intervallo di celle adiacenti in base ai dati attuali) Altre formule nella cartella di lavoro non saranno calcolate ricorsivamente anche se sono state utilizzate dalle formule di array dinamici. |
| [RefreshDynamicArrayFormulas_Bool_CalculationOptions](./refreshdynamicarrayformulas_bool_calculationoptions/) | Aggiorna le formule di array dinamici (espansione in un nuovo intervallo di celle adiacenti in base ai dati attuali) |
| [GetDefaultStyle](./getdefaultstyle/) | Ottiene o imposta l'oggetto Style predefinito della cartella di lavoro. |
| [SetDefaultStyle](./setdefaultstyle/) | Ottiene o imposta l'oggetto Style predefinito della cartella di lavoro. |
| [GetMatchingColor](./getmatchingcolor/) | Trova il colore più corrispondente nella tavolozza corrente. |
| [IsDigitallySigned](./isdigitallysigned/) | Indica se questo foglio di calcolo è firmato digitalmente. |
| [SetEncryptionOptions](./setencryptionoptions/) | Imposta le opzioni di crittografia. |
| [Protect](./protect/) | Protegge una cartella di lavoro. |
| [ProtectSharedWorkbook](./protectsharedworkbook/) | Protegge una cartella di lavoro condivisa. |
| [Unprotect](./unprotect/) | Rimuove la protezione da una cartella di lavoro. |
| [UnprotectSharedWorkbook](./unprotectsharedworkbook/) | Rimuove la protezione da una cartella di lavoro condivisa. |
| [IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | Indica se la struttura o la finestra è protetta da password. |
| [RemoveMacro](./removemacro/) | Rimuove VBA/macro da questo foglio di calcolo. |
| [GetVbaProject](./getvbaproject/) | Ottiene il VbaProject in un foglio di calcolo. |
| [RemoveDigitalSignature](./removedigitalsignature/) | Rimuove la firma digitale da questo foglio di calcolo. |
| [AcceptAllRevisions](./acceptallrevisions/) | Accetta tutte le modifiche tracciate nella cartella di lavoro. |
| [GetHasMacro](./gethasmacro/) | Indica se questo foglio di calcolo contiene macro/VBA. |
| [GetHasRevisions](./gethasrevisions/) | Ottiene se la cartella di lavoro ha modifiche tracciate |
| [GetFileName](./getfilename/) | Ottiene e imposta il nome file corrente. |
| [SetFileName](./setfilename/) | Ottiene e imposta il nome file corrente. |
| [GetDataSorter](./getdatasorter/) | Ottiene un oggetto DataSorter per ordinare i dati. |
| [GetThemeColor](./getthemecolor/) | Ottiene il colore del tema. |
| [SetThemeColor](./setthemecolor/) | Imposta il colore del tema |
| [GetTheme](./gettheme/) | Ottiene il nome del tema. |
| [CustomTheme](./customtheme/) | Personalizza il tema. |
| [CopyTheme](./copytheme/) | Copia il tema da un altro foglio di lavoro. |
| [UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | Aggiorna la definizione delle funzioni personalizzate. |
| [UpdateLinkedDataSource](./updatelinkeddatasource/) | Se questo foglio di lavoro contiene collegamenti esterni a un'altra fonte di dati, Aspose.Cells cercherà di recuperare i dati più recenti dalle fonti fornite. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Restituisce una raccolta DocumentProperty che rappresenta tutte le proprietà di documento integrate del foglio di calcolo. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Restituisce una raccolta DocumentProperty che rappresenta tutte le proprietà di documento personalizzate del foglio di calcolo. |
| [GetFileFormat](./getfileformat/) | Ottiene e imposta il formato del file. |
| [SetFileFormat](./setfileformat/) | Ottiene e imposta il formato del file. |
| [GetHasCustomFunction](./gethascustomfunction/) | Rileva se in questo foglio di lavoro è utilizzata una funzione personalizzata, ad esempio nelle formule delle celle o nei nomi definiti... |
| [GetInterruptMonitor](./getinterruptmonitor/) | Ottiene e imposta il monitor di interruzione. |
| [SetInterruptMonitor_AbstractInterruptMonitor](./setinterruptmonitor_abstractinterruptmonitor/) | Ottiene e imposta il monitor di interruzione. |
| [SetInterruptMonitor_InterruptMonitor](./setinterruptmonitor_interruptmonitor/) | Imposta il monitor di interruzione. |
| [GetContentTypeProperties](./getcontenttypeproperties/) | Ottiene l'elenco degli oggetti ContentTypeProperty nel foglio di lavoro. |
| [GetCustomXmlParts](./getcustomxmlparts/) | Rappresenta una parte di archiviazione dati XML personalizzata (dati XML personalizzati all'interno di un pacchetto). |
| [GetDataMashup](./getdatamashup/) | Ottiene i dati mashup. |
| [GetRibbonXml](./getribbonxml/) | Ottiene e imposta il file XML che definisce l'interfaccia Ribbon. |
| [SetRibbonXml](./setribbonxml/) | Ottiene e imposta il file XML che definisce l'interfaccia Ribbon. |
| [GetAbsolutePath](./getabsolutepath/) | Ottiene e imposta il percorso assoluto del file. |
| [SetAbsolutePath](./setabsolutepath/) | Ottiene e imposta il percorso assoluto del file. |
| [GetDataConnections](./getdataconnections/) | Ottiene la raccolta ExternalConnection. |
| [ImportXml_String_String_Int_Int](./importxml_string_string_int_int/) | Importa/Aggiorna un file di dati XML nel foglio di lavoro. |
| [ImportXml_Stream_String_Int_Int](./importxml_stream_string_int_int/) | Importa/Aggiorna un file di dati XML nel foglio di lavoro. |
| [ExportXml_String_String](./exportxml_string_string/) | Esporta i dati XML collegati alla mappa XML specificata. |
| [ExportXml_String](./exportxml_string/) | Esporta dati XML. |
| [SetDigitalSignature](./setdigitalsignature/) | Imposta la firma digitale a un file di foglio di calcolo (Excel2007 e versioni successive). |
| [AddDigitalSignature](./adddigitalsignature/) | Aggiunge la firma digitale a un file di foglio di calcolo OOXML (Excel2007 e versioni successive). |
| [GetDigitalSignature](./getdigitalsignature/) | Ottiene la firma digitale dal file. |
| [RemovePersonalInformation](./removepersonalinformation/) | Rimuove le informazioni personali. |
| [GetDataModel](./getdatamodel/) | Ottiene il modello di dati nel foglio di lavoro. |
| [RefreshAll](./refreshall/) | Aggiorna le forme collegate, tutte le tabelle pivot e i grafici con l'origine pivot. |
| [Dispose](./dispose/) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino delle risorse non gestite. |
