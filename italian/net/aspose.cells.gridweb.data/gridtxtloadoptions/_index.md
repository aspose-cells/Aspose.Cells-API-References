---
title: "Classe GridTxtLoadOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridTxtLoadOptions. Rappresenta le opzioni per il caricamento di file di testo"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridtxtloadoptions/
---
## GridTxtLoadOptions class

Rappresenta le opzioni per il caricamento di file di testo.

```csharp
[Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.TxtLoadOptions ")]
public class GridTxtLoadOptions : GridLoadOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [GridTxtLoadOptions](gridtxtloadoptions/)() | Crea le opzioni per il caricamento di un file di testo. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Indica se filtrare automaticamente i dati durante il caricamento dei file. (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Verifica se i dati sono validi nel file modello. (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file Excel quando l'utente modifica gli oggetti correlati alle celle. Ad esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true, otterrai un'eccezione. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare il valore completo per altri formati di file come CSV. Tuttavia, se hai impostato un valore non valido per il formato Excel, non dovresti salvare la cartella di lavoro come file Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato. (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertdatetimedata/) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati di tipo data. |
| [ConvertNumericData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertnumericdata/) { get; set; } | Ottiene o imposta un valore che indica se la stringa nel file di testo viene convertita in dati numerici. |
| [Encoding](../../aspose.cells.gridweb.data/gridtxtloadoptions/encoding/) { get; set; } | Ottiene e imposta la codifica predefinita. Si applica solo ai file csv. |
| [ExtendToNextSheet](../../aspose.cells.gridweb.data/gridtxtloadoptions/extendtonextsheet/) { get; set; } | Indica se estendere i dati al foglio successivo quando le righe o le colonne superano il limite. Se questa proprietà è true, i dati aggiuntivi saranno spostati al foglio successivo rispetto a quello corrente (se il foglio corrente è l'ultimo, verrà aggiunto un nuovo foglio alla cartella di lavoro). Se la proprietà è false, i dati che superano il limite verranno ignorati. Il valore predefinito è false; |
| [HasFormula](../../aspose.cells.gridweb.data/gridtxtloadoptions/hasformula/) { get; set; } | Indica se il testo è una formula se inizia con "=\". |
| [HasTextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/hastextqualifier/) { get; set; } | Indica se è presente un qualificatore di testo per il valore della cella. Il valore predefinito è true. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Ignora i dati non stampati se si stampa direttamente il file (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [IsMultiEncoded](../../aspose.cells.gridweb.data/gridtxtloadoptions/ismultiencoded/) { get; set; } | True indica che il file contiene diverse codifiche. |
| [KeepPrecision](../../aspose.cells.gridweb.data/gridtxtloadoptions/keepprecision/) { get; set; } | Indica se non analizzare un valore stringa se la lunghezza è 15. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Indica se mantenere i dati non analizzati in memoria per la cartella di lavoro quando viene caricata dal file modello. Il valore predefinito è true. (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Indica se adattare solo le righe la cui altezza non è personalizzata. (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Indica se analizzare la formula durante la lettura del file. (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Indica se analizzare i record memorizzati nella cache della pivot durante il caricamento del file. Il valore predefinito è false. (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Ottiene e imposta la password della cartella di lavoro. (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Indica se conservare gli spazi e le interruzioni di riga inseriti tra i token della formula durante il recupero e l'impostazione delle formule. Il valore predefinito è false. (Ereditato da [`GridLoadOptions`](../gridloadoptions/).) |
| [Separator](../../aspose.cells.gridweb.data/gridtxtloadoptions/separator/) { get; set; } | Ottiene e imposta il separatore di caratteri del file di testo. |
| [SeparatorString](../../aspose.cells.gridweb.data/gridtxtloadoptions/separatorstring/) { get; set; } | Ottiene e imposta un valore stringa come separatore. |
| [TextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/textqualifier/) { get; set; } | Specifica il qualificatore di testo per i valori delle celle. Il qualificatore predefinito è '\"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Indica se i delimitatori consecutivi devono essere trattati come uno. |
| [TreatQuotePrefixAsValue](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatquoteprefixasvalue/) { get; set; } | Indica se il segno di apice singolo iniziale deve essere considerato parte del valore di una cella. Il valore predefinito è true. Se è false, l'apice singolo iniziale verrà rimosso dal valore della cella corrispondente e [`QuotePrefix`](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) sarà impostato su true per la cella. |

### Vedi anche

* class [GridLoadOptions](../gridloadoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


