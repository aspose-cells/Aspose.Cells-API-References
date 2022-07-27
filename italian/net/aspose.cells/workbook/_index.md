---
title: Workbook
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta un oggetto radice per creare un foglio di calcolo Excel.
type: docs
weight: 6480
url: /it/net/aspose.cells/workbook/
---
## Workbook class

Rappresenta un oggetto radice per creare un foglio di calcolo Excel.

```csharp
public class Workbook : IDisposable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Workbook](workbook#constructor)() | Inizializza una nuova istanza di[`Workbook`](../workbook) classe. |
| [Workbook](workbook#constructor_1)(FileFormatType) | Inizializza una nuova istanza di[`Workbook`](../workbook) classe. |
| [Workbook](workbook#constructor_2)(Stream) | Inizializza una nuova istanza di[`Workbook`](../workbook) classe e apri uno stream. |
| [Workbook](workbook#constructor_4)(string) | Inizializza una nuova istanza di[`Workbook`](../workbook) classe e apri un file. |
| [Workbook](workbook#constructor_3)(Stream, LoadOptions) | Inizializza una nuova istanza di[`Workbook`](../workbook) classe e apri stream. |
| [Workbook](workbook#constructor_5)(string, LoadOptions) | Inizializza una nuova istanza di[`Workbook`](../workbook) classe e apri un file. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath) { get; set; } | Ottiene e imposta il percorso assoluto del file. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties) { get; } | Restituisce a[`DocumentProperty`](../../aspose.cells.properties/documentproperty)raccolta che rappresenta tutte le proprietà del documento integrate nel foglio di calcolo. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory) { get; } | Ottiene la factory per la creazione di ICellsDataTable da oggetti personalizzati |
| [Colors](../../aspose.cells/workbook/colors) { get; } | Restituisce i colori nella tavolozza per il foglio di calcolo. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties) { get; } | Ottiene l'elenco di[`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty) oggetti nella cartella di lavoro. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool) { get; } | Ottiene il numero degli stili nel pool di stili. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties) { get; } | Restituisce a[`DocumentProperty`](../../aspose.cells.properties/documentproperty) raccolta che rappresenta tutte le proprietà del documento personalizzato del foglio di calcolo. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts) { get; } | Rappresenta una parte di archiviazione dati XML personalizzata (dati XML personalizzati all'interno di un pacchetto). |
| [DataConnections](../../aspose.cells/workbook/dataconnections) { get; } | Ottiene il[`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection) raccolta. |
| [DataMashup](../../aspose.cells/workbook/datamashup) { get; } | Ottiene dati mashup. |
| [DataSorter](../../aspose.cells/workbook/datasorter) { get; } | Ottiene un oggetto DataSorter per ordinare i dati. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle) { get; set; } | Ottiene o imposta il valore predefinito[`Style`](../style) oggetto della cartella di lavoro. |
| [FileFormat](../../aspose.cells/workbook/fileformat) { get; set; } | Ottiene e imposta il formato del file. |
| [FileName](../../aspose.cells/workbook/filename) { get; set; } | Ottiene e imposta il nome del file corrente. |
| [HasMacro](../../aspose.cells/workbook/hasmacro) { get; } | Indica se questo foglio di calcolo contiene macro/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions) { get; } | Ottiene se la cartella di lavoro contiene modifiche rilevate |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor) { get; set; } | Ottiene e imposta il monitor di interruzione. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned) { get; } | Indica se questo foglio di calcolo è firmato digitalmente. |
| [IsLicensed](../../aspose.cells/workbook/islicensed) { get; } | Indica se la licenza è impostata. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword) { get; } | Indica se la struttura o la finestra sono protette con password. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml) { get; set; } | Ottiene e imposta il file XML che definisce l'interfaccia utente della barra multifunzione. |
| [Settings](../../aspose.cells/workbook/settings) { get; } | Rappresenta le impostazioni della cartella di lavoro. |
| [Theme](../../aspose.cells/workbook/theme) { get; } | Ottiene il nome del tema. |
| [VbaProject](../../aspose.cells/workbook/vbaproject) { get; } | Ottiene il[`VbaProject`](./vbaproject) in un foglio di calcolo. |
| [Worksheets](../../aspose.cells/workbook/worksheets) { get; } | Ottiene il[`WorksheetCollection`](../worksheetcollection) raccolta nel foglio di calcolo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions)() | Accetta tutte le modifiche rilevate nella cartella di lavoro. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature)(DigitalSignatureCollection) | Aggiunge la firma digitale a un file di foglio di calcolo OOXML (Excel2007 e versioni successive). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula)() | Calcola il risultato delle formule. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_2)(bool) | Calcola il risultato delle formule. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_1)(CalculationOptions) | Calcolo delle formule in questa cartella di lavoro. |
| [ChangePalette](../../aspose.cells/workbook/changepalette)(Color, int) | Modifica la tavolozza per il foglio di calcolo nell'indice specificato. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache)(AccessCacheOptions) | Chiude la sessione che utilizza le cache per accedere ai dati. |
| [Combine](../../aspose.cells/workbook/combine)(Workbook) | Combina un altro oggetto cartella di lavoro. |
| [Copy](../../aspose.cells/workbook/copy#copy)(Workbook) | Copia i dati da un oggetto cartella di lavoro di origine. |
| [Copy](../../aspose.cells/workbook/copy#copy_1)(Workbook, CopyOptions) | Copia i dati da un oggetto cartella di lavoro di origine. |
| [CopyTheme](../../aspose.cells/workbook/copytheme)(Workbook) | Copia il tema da un'altra cartella di lavoro. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle)(BuiltinStyleType) | Crea uno stile integrato in base al tipo specificato. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor)() | Crea a[`CellsColor`](../cellscolor) oggetto. |
| [CreateStyle](../../aspose.cells/workbook/createstyle)() | Crea un nuovo stile. |
| [CustomTheme](../../aspose.cells/workbook/customtheme)(string, Color[]) | Personalizza il tema. |
| [Dispose](../../aspose.cells/workbook/dispose)() | Esegue attività definite dall'applicazione associate alla liberazione, rilascio o ripristino di risorse non gestite. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml)(string, Stream) | Esporta dati XML. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml_1)(string, string) | Esporta dati XML collegati dalla mappa XML specificata. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature)() | Ottiene la firma digitale dal file. |
| [GetFonts](../../aspose.cells/workbook/getfonts)() | Ottiene tutti i caratteri nel pool di stili. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor)(Color) | Trova il colore più adatto nella tavolozza corrente. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle)(string) | Ottiene lo stile denominato nel pool di stili. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool)(int) | Ottiene lo stile nel pool di stili. Tutti gli stili nella cartella di lavoro verranno raccolti in un pool. Nelle celle è presente solo un semplice indice di riferimento. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor)(ThemeColorType) | Ottiene il colore del tema. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml)(Stream, string, int, int) | Importa/aggiorna un file di dati XML nella cartella di lavoro. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml_1)(string, string, int, int) | Importa/aggiorna un file di dati XML nella cartella di lavoro. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette)(Color) | Verifica se nella tavolozza del foglio di calcolo è presente un colore. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas)(bool) | Analizza tutte le formule che non sono state analizzate quando sono state caricate dal file modello o impostate su una cella. |
| [Protect](../../aspose.cells/workbook/protect)(ProtectionType, string) | Protegge una cartella di lavoro. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook)(string) | Protegge una cartella di lavoro condivisa. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas)(bool) | Aggiorna le formule di matrice dinamica (si riversa in un nuovo intervallo di celle adiacenti in base ai dati correnti) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature)() | Rimuove la firma digitale da questo foglio di lavoro. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro)() | Rimuove VBA/macro da questo foglio di calcolo. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation)() | Rimuove le informazioni personali. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles)() | Rimuovi tutti gli stili non utilizzati. |
| [Replace](../../aspose.cells/workbook/replace#replace)(bool, object) | Sostituisce i valori delle celle con nuovi dati. |
| [Replace](../../aspose.cells/workbook/replace#replace_1)(int, object) | Sostituisce i valori delle celle con nuovi dati. |
| [Replace](../../aspose.cells/workbook/replace#replace_6)(string, DataTable) | Sostituisce i valori delle celle con i dati di aDataTable . |
| [Replace](../../aspose.cells/workbook/replace#replace_2)(string, double) | Sostituisce il valore di una cella con un nuovo double. |
| [Replace](../../aspose.cells/workbook/replace#replace_4)(string, int) | Sostituisce il valore di una cella con un nuovo intero. |
| [Replace](../../aspose.cells/workbook/replace#replace_7)(string, string) | Sostituisce il valore di una cella con una nuova stringa. |
| [Replace](../../aspose.cells/workbook/replace#replace_3)(string, double[], bool) | Sostituisce i valori delle celle con un doppio array. |
| [Replace](../../aspose.cells/workbook/replace#replace_5)(string, int[], bool) | Sostituisce i valori delle celle con un array intero. |
| [Replace](../../aspose.cells/workbook/replace#replace_8)(string, string, ReplaceOptions) | Sostituisce il valore di una cella con una nuova stringa. |
| [Replace](../../aspose.cells/workbook/replace#replace_9)(string, string[], bool) | Sostituisce il valore di una cella con un nuovo array di stringhe. |
| [Save](../../aspose.cells/workbook/save#save_2)(string) | Salva la cartella di lavoro sul disco. |
| [Save](../../aspose.cells/workbook/save#save)(Stream, SaveFormat) | Salva la cartella di lavoro nello stream. |
| [Save](../../aspose.cells/workbook/save#save_1)(Stream, SaveOptions) | Salva la cartella di lavoro nello stream. |
| [Save](../../aspose.cells/workbook/save#save_3)(string, SaveFormat) | Salva la cartella di lavoro sul disco. |
| [Save](../../aspose.cells/workbook/save#save_4)(string, SaveOptions) | Salva la cartella di lavoro sul disco. |
| [Save](../../aspose.cells/workbook/save#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Crea il foglio di calcolo dei risultati e lo trasferisce al client, quindi lo apre nel browser o nella cartella di lavoro MS. |
| [Save](../../aspose.cells/workbook/save#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Crea il foglio di calcolo dei risultati e lo trasferisce al client, quindi lo apre nel browser o nella cartella di lavoro MS. |
| [SaveToStream](../../aspose.cells/workbook/savetostream)() | Salva il file Excel in un oggetto MemoryStream e lo restituisce. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature)(DigitalSignatureCollection) | Imposta la firma digitale su un file di foglio di calcolo (Excel2007 e versioni successive). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions)(EncryptionType, int) | Imposta opzioni di crittografia. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor)(ThemeColorType, Color) | Imposta il colore del tema |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache)(AccessCacheOptions) | Avvia la sessione che utilizza le cache per accedere ai dati. |
| [Unprotect](../../aspose.cells/workbook/unprotect)(string) | Annulla la protezione di una cartella di lavoro. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook)(string) | Annulla la protezione di una cartella di lavoro condivisa. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource)(Workbook[]) | Se questa cartella di lavoro contiene collegamenti esterni ad altre origini dati, Aspose.Cells tenterà di recuperare i dati più recenti. |

### Osservazioni

La classe Workbook denota un foglio di calcolo Excel. Ogni foglio di calcolo può contenere più fogli di lavoro. La funzionalità di base della classe è aprire e salvare file excel nativi. La classe ha alcune funzionalità avanzate come la copia di dati da altre cartelle di lavoro, la combinazione di due cartelle di lavoro e la protezione del foglio di calcolo Excel.

### Esempi

L'esempio seguente carica una cartella di lavoro da un file denominato designer.xls e rende invisibili le barre di scorrimento orizzontale e verticale per la cartella di lavoro. Quindi sostituisce due valori di stringa rispettivamente con un valore intero e un valore di stringa all'interno del foglio di calcolo e infine invia il file aggiornato al browser del client.

```csharp
[C#]

//Apri un file di progettazione
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

//Imposta le barre di scorrimento
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

//Sostituisci la stringa segnaposto con nuovi valori
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'Apri un file di progettazione
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'Imposta le barre di scorrimento
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'Sostituisci la stringa segnaposto con nuovi valori
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
