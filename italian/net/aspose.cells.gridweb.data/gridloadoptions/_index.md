---
title: "Classe GridLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridWeb.Data.GridLoadOptions classe. Rappresenta le opzioni di caricamento del file. Obsoleto: questa classe sarà resa obsoleta dopo l'uso stand‑alone della DLL dell'API pubblica di cells; invece è possibile utilizzare Aspose.Cells.LodOptions"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridloadoptions/
---
## GridLoadOptions class

Rappresenta le opzioni di caricamento del file. [Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions ")]

```csharp
public class GridLoadOptions : ISerializable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridLoadOptions](gridloadoptions/)() | Crea un'opzione per il caricamento del file. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file. |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Verifica se i dati sono validi nel file modello. |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true otterrai un'Exception. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato file excel, non dovresti salvare la workbook in formato excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file excel generato. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Ignora i dati che non vengono stampati se si stampa direttamente il file |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Indica se mantenere i dati non analizzati in memoria per il Workbook quando viene caricato da un file modello. Il valore predefinito è true. |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Indica se adattare solo le righe la cui altezza non è personalizzata. |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Indica se analizzare la formula durante la lettura del file. |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Indica se analizzare i record della cache pivot durante il caricamento del file. Il valore predefinito è false. |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Ottiene e imposta la password del workbook. |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Indica se preservare quegli spazi e interruzioni di riga inseriti tra i token della formula durante l'ottenimento e l'impostazione delle formule. Il valore predefinito è false. |

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


