---
title: "Classe Workbook"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Workbook. Rappresenta un oggetto radice per creare un foglio di calcolo Excel"
type: docs
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
| [Workbook](workbook/#constructor)() | Inizializza una nuova istanza della classe `Workbook`. |
| [Workbook](workbook/#constructor_1)(FileFormatType) | Inizializza una nuova istanza della classe `Workbook`. |
| [Workbook](workbook/#constructor_2)(LoadOptions) | Inizializza una nuova istanza vuota della classe `Workbook` con opzioni |
| [Workbook](workbook/#constructor_3)(Stream) | Inizializza una nuova istanza della classe `Workbook` e apre un flusso. |
| [Workbook](workbook/#constructor_5)(string) | Inizializza una nuova istanza della classe `Workbook` e apre un file. |
| [Workbook](workbook/#constructor_4)(Stream, LoadOptions) | Inizializza una nuova istanza della classe `Workbook` e apre lo stream. |
| [Workbook](workbook/#constructor_6)(string, LoadOptions) | Inizializza una nuova istanza della classe `Workbook` e apre un file. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath/) { get; set; } | Ottiene e imposta il percorso assoluto del file. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties/) { get; } | Restituisce una collezione di [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà di documento integrate del foglio elettronico. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory/) { get; } | Ottiene la factory per costruire ICellsDataTable da oggetti personalizzati |
| [Colors](../../aspose.cells/workbook/colors/) { get; } | Restituisce i colori nella tavolozza per il foglio di calcolo. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties/) { get; } | Ottiene l'elenco degli oggetti [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty/) nel workbook. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool/) { get; } | Ottiene il numero degli stili nel pool di stili. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties/) { get; } | Restituisce una collezione di [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) che rappresenta tutte le proprietà di documento personalizzate del foglio elettronico. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts/) { get; } | Rappresenta una parte di archiviazione dati XML personalizzata (dati XML personalizzati all'interno di un pacchetto). |
| [DataConnections](../../aspose.cells/workbook/dataconnections/) { get; } | Ottiene la collezione [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection/). |
| [DataMashup](../../aspose.cells/workbook/datamashup/) { get; } | Ottiene i dati mashup. |
| [DataModel](../../aspose.cells/workbook/datamodel/) { get; } | Ottiene il modello dati nel workbook. |
| [DataSorter](../../aspose.cells/workbook/datasorter/) { get; } | Ottiene un oggetto DataSorter per ordinare i dati. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle/) { get; set; } | Ottiene o imposta l'oggetto [`Style`](../style/) predefinito del workbook. |
| [FileFormat](../../aspose.cells/workbook/fileformat/) { get; set; } | Ottiene e imposta il formato del file. |
| [FileName](../../aspose.cells/workbook/filename/) { get; set; } | Ottiene e imposta il nome file corrente. |
| [HasCustomFunction](../../aspose.cells/workbook/hascustomfunction/) { get; } | Rileva se nel workbook è presente una funzione personalizzata, ad esempio nella formula di una cella o nei nomi definiti... |
| [HasMacro](../../aspose.cells/workbook/hasmacro/) { get; } | Indica se questo foglio di calcolo contiene macro/VBA. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions/) { get; } | Ottiene se il workbook ha modifiche tracciate |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor/) { get; set; } | Ottiene e imposta il monitor di interruzione. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned/) { get; } | Indica se questo foglio di calcolo è firmato digitalmente. |
| [IsLicensed](../../aspose.cells/workbook/islicensed/) { get; } | Indica se la licenza è impostata. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword/) { get; } | Indica se la struttura o la finestra è protetta da password. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml/) { get; set; } | Ottiene e imposta il file XML che definisce l'interfaccia Ribbon UI. |
| [Settings](../../aspose.cells/workbook/settings/) { get; } | Rappresenta le impostazioni del workbook. |
| [Theme](../../aspose.cells/workbook/theme/) { get; } | Ottiene il nome del tema. |
| [VbaProject](../../aspose.cells/workbook/vbaproject/) { get; } | Ottiene il [`VbaProject`](./vbaproject/) in un foglio di calcolo. |
| [Worksheets](../../aspose.cells/workbook/worksheets/) { get; } | Ottiene la collezione [`WorksheetCollection`](../worksheetcollection/) nel foglio di calcolo. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions/)() | Accetta tutte le modifiche tracciate nella cartella di lavoro. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature/)(DigitalSignatureCollection) | Aggiunge la firma digitale a un file di foglio di calcolo OOXML (Excel2007 e versioni successive). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula)() | Calcola il risultato delle formule. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_2)(bool) | Calcola il risultato delle formule. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_1)(CalculationOptions) | Calcolo delle formule in questa cartella di lavoro. |
| [ChangePalette](../../aspose.cells/workbook/changepalette/)(Color, int) | Modifica la tavolozza per il foglio di calcolo nell'indice specificato. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache/)(AccessCacheOptions) | Chiude la sessione che utilizza cache per accedere ai dati. |
| [Combine](../../aspose.cells/workbook/combine/)(Workbook) | Combina un altro oggetto Workbook. |
| [Copy](../../aspose.cells/workbook/copy/#copy)(Workbook) | Copia i dati da un oggetto Workbook di origine. |
| [Copy](../../aspose.cells/workbook/copy/#copy_1)(Workbook, CopyOptions) | Copia un altro oggetto Workbook. |
| [CopyTheme](../../aspose.cells/workbook/copytheme/)(Workbook) | Copia il tema da un'altra cartella di lavoro. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle/)(BuiltinStyleType) | Crea uno stile predefinito del tipo specificato. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor/)() | Crea un oggetto [`CellsColor`](../cellscolor/). |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle)() | Crea un nuovo stile. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle_1)(bool) | Crea un nuovo stile. |
| [CustomTheme](../../aspose.cells/workbook/customtheme/)(string, Color[]) | Personalizza il tema. |
| [Dispose](../../aspose.cells/workbook/dispose/)() | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al reset delle risorse non gestite. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml)(string, Stream) | Esporta dati XML. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml_1)(string, string) | Esporta i dati XML collegati dalla mappa XML specificata. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature/)() | Ottiene la firma digitale dal file. |
| [GetFonts](../../aspose.cells/workbook/getfonts/)() | Ottiene tutti i caratteri nel pool di stili. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor/)(Color) | Trova il colore più corrispondente nella tavolozza corrente. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle/)(string) | Ottiene lo stile denominato nel pool di stili. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool/)(int) | Ottiene lo stile nel pool di stili. Tutti gli stili nella cartella di lavoro saranno raccolti in un pool. Nelle celle è presente solo un semplice indice di riferimento. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor/)(ThemeColorType) | Ottiene il colore del tema. |
| [HasExernalLinks](../../aspose.cells/workbook/hasexernallinks/)() | (**Obsolete.**) Indica se questa cartella di lavoro contiene collegamenti esterni ad altre fonti di dati. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml)(Stream, string, int, int) | Importa/Aggiorna un file di dati XML nella cartella di lavoro. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml_1)(string, string, int, int) | Importa/Aggiorna un file di dati XML nella cartella di lavoro. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette/)(Color) | Verifica se un colore è nella tavolozza per il foglio di calcolo. |
| [MergeNamedStyles](../../aspose.cells/workbook/mergenamedstyles/)(Workbook) | Unisce gli stili denominati dall'altro file Excel. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas/)(bool) | Analizza tutte le formule che non sono state analizzate quando sono state caricate dal file modello o impostate in una cella. |
| [Protect](../../aspose.cells/workbook/protect/)(ProtectionType, string) | Protegge una cartella di lavoro. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook/)(string) | Protegge una cartella di lavoro condivisa. |
| [RefreshAll](../../aspose.cells/workbook/refreshall/)() | Aggiorna le forme collegate, tutte le tabelle pivot e i grafici con la fonte pivot. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas)(bool) | Aggiorna le formule di array dinamici (si estendono in un nuovo intervallo di celle adiacenti in base ai dati attuali). Altre formule nella cartella di lavoro non saranno calcolate ricorsivamente anche se sono state utilizzate dalle formule di array dinamici. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas_1)(bool, CalculationOptions) | Aggiorna le formule di array dinamici (si estendono in un nuovo intervallo di celle adiacenti in base ai dati attuali). |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature/)() | Rimuove la firma digitale da questo foglio di calcolo. |
| [RemoveExternalLinks](../../aspose.cells/workbook/removeexternallinks/)() | (**Obsolete.**) Rimuove tutti i collegamenti esterni nella cartella di lavoro. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro/)() | Rimuove VBA/macro da questo foglio di calcolo. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation/)() | Rimuove le informazioni personali. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles/)() | Rimuove tutti gli stili inutilizzati. |
| [Replace](../../aspose.cells/workbook/replace/#replace)(bool, object) | Sostituisce i valori delle celle con nuovi dati. |
| [Replace](../../aspose.cells/workbook/replace/#replace_1)(int, object) | Sostituisce i valori delle celle con nuovi dati. |
| [Replace](../../aspose.cells/workbook/replace/#replace_6)(string, DataTable) | Sostituisce i valori delle celle con i dati da una DataTable. |
| [Replace](../../aspose.cells/workbook/replace/#replace_2)(string, double) | Sostituisce il valore di una cella con un nuovo double. |
| [Replace](../../aspose.cells/workbook/replace/#replace_4)(string, int) | Sostituisce il valore di una cella con un nuovo intero. |
| [Replace](../../aspose.cells/workbook/replace/#replace_7)(string, string) | Sostituisce il valore di una cella con una nuova stringa. |
| [Replace](../../aspose.cells/workbook/replace/#replace_3)(string, double[], bool) | Sostituisce i valori delle celle con un array di double. |
| [Replace](../../aspose.cells/workbook/replace/#replace_5)(string, int[], bool) | Sostituisce i valori delle celle con un array di interi. |
| [Replace](../../aspose.cells/workbook/replace/#replace_8)(string, string, ReplaceOptions) | Sostituisce il valore di una cella con una nuova stringa. |
| [Replace](../../aspose.cells/workbook/replace/#replace_9)(string, string[], bool) | Sostituisce il valore di una cella con un nuovo array di stringhe. |
| [Save](../../aspose.cells/workbook/save/#save_2)(string) | Salva la cartella di lavoro su disco. |
| [Save](../../aspose.cells/workbook/save/#save)(Stream, SaveFormat) | Salva la cartella di lavoro sullo stream. |
| [Save](../../aspose.cells/workbook/save/#save_1)(Stream, SaveOptions) | Salva la cartella di lavoro sullo stream. |
| [Save](../../aspose.cells/workbook/save/#save_3)(string, SaveFormat) | Salva la cartella di lavoro su disco. |
| [Save](../../aspose.cells/workbook/save/#save_4)(string, SaveOptions) | Salva la cartella di lavoro su disco. |
| [Save](../../aspose.cells/workbook/save/#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Crea il foglio di calcolo risultato e lo trasferisce al client, quindi lo apre nel browser o in MS Workbook. |
| [Save](../../aspose.cells/workbook/save/#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Crea il foglio di calcolo risultato e lo trasferisce al client, quindi lo apre nel browser o in MS Workbook. |
| [SaveToStream](../../aspose.cells/workbook/savetostream/)() | Salva il file Excel in un oggetto MemoryStream come file xls Excel97-2003 e lo restituisce. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature/)(DigitalSignatureCollection) | Imposta la firma digitale su un file di foglio di calcolo (Excel2007 e versioni successive). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions/)(EncryptionType, int) | Imposta le opzioni di crittografia. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor/)(ThemeColorType, Color) | Imposta il colore del tema |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache/)(AccessCacheOptions) | Avvia la sessione che utilizza cache per accedere ai dati. |
| [Unprotect](../../aspose.cells/workbook/unprotect/)(string) | Rimuove la protezione da una cartella di lavoro. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook/)(string) | Rimuove la protezione da una cartella di lavoro condivisa. |
| [UpdateCustomFunctionDefinition](../../aspose.cells/workbook/updatecustomfunctiondefinition/)(CustomFunctionDefinition) | Aggiorna la definizione delle funzioni personalizzate. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource/)(Workbook[]) | Se questa cartella di lavoro contiene collegamenti esterni a un'altra fonte di dati, Aspose.Cells cercherà di recuperare i dati più recenti dalle fonti fornite. |

### Osservazioni

La classe Workbook indica un foglio di calcolo Excel. Ogni foglio di calcolo può contenere più fogli di lavoro. La funzionalità di base della classe è aprire e salvare file Excel nativi. La classe dispone di alcune funzionalità avanzate come copiare dati da altri Workbook, combinare due Workbook, convertire Excel in PDF, renderizzare Excel in immagine e proteggere il foglio di calcolo Excel.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDemo
    {
        public static void WorkbookExample()
        {
            // Crea una nuova istanza di Workbook
            Workbook workbook = new Workbook();

            // Accedi al foglio di lavoro predefinito
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcune proprietà della cartella di lavoro
            workbook.FileName = "ExampleWorkbook.xlsx";
            workbook.DefaultStyle.Font.Name = "Tahoma";

            // Aggiungi un nuovo foglio di lavoro
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = "NewSheet";

            // Aggiungi alcuni dati al nuovo foglio di lavoro
            newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");

            // Imposta alcune proprietà del documento
            workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
            workbook.CustomDocumentProperties.Add("Checked by", "Jane");

            // Salva la cartella di lavoro in un file
            workbook.Save("WorkbookExample.xlsx");

            // Visualizza alcune proprietà
            Console.WriteLine("Workbook File Name: " + workbook.FileName);
            Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);

            // Verifica se la cartella di lavoro è licenziata
            Console.WriteLine("Is Licensed: " + workbook.IsLicensed);

            // Verifica se la cartella di lavoro è firmata digitalmente
            Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);

            // Verifica se la cartella di lavoro contiene macro
            Console.WriteLine("Has Macros: " + workbook.HasMacro);

            // Verifica se la cartella di lavoro ha modifiche tracciate
            Console.WriteLine("Has Revisions: " + workbook.HasRevisions);

            // Verifica il numero di stili nel pool di stili
            Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);

            // Verifica il nome del tema
            Console.WriteLine("Theme: " + workbook.Theme);

            // Verifica se la cartella di lavoro è protetta da una password
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Verifica se la cartella di lavoro contiene collegamenti esterni
            Console.WriteLine("Has External Links: " + (workbook.Worksheets.ExternalLinks.Count > 0));

            // Elimina la cartella di lavoro
            workbook.Dispose();
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


