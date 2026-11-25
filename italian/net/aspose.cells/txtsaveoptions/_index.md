---
title: "Classe TxtSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.TxtSaveOptions classe. Rappresenta le opzioni di salvataggio per il formato testo csv/tab delimitato/altro"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/
---
## TxtSaveOptions class

Rappresenta le opzioni di salvataggio per il formato csv/tab delimitato/altri formati di testo.

```csharp
public class TxtSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TxtSaveOptions](txtsaveoptions/#constructor)() | Crea le opzioni di salvataggio del file di testo. |
| [TxtSaveOptions](txtsaveoptions/#constructor_1)(SaveFormat) | Crea le opzioni di salvataggio del file di testo. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlwaysQuoted](../../aspose.cells/txtsaveoptions/alwaysquoted/) { get; set; } | (**Obsolete.**) Indica se aggiungere sempre '"' per ogni campo. Se vero, tutti i valori saranno racchiusi tra virgolette; se falso, i valori saranno racchiusi tra virgolette solo quando necessario (ad esempio, quando i valori contengono caratteri speciali come '"', '\n' o il carattere separatore). Il valore predefinito è false. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi il workbook vuoto dopo aver salvato il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/txtsaveoptions/encoding/) { get; set; } | Ottiene e imposta la codifica predefinita. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ExportAllSheets](../../aspose.cells/txtsaveoptions/exportallsheets/) { get; set; } | Indica se esportare tutti i fogli nel file di testo. Se è false, esporta solo il foglio attivo, proprio come MS Excel. |
| [ExportArea](../../aspose.cells/txtsaveoptions/exportarea/) { get; set; } | Intervallo di celle da esportare. |
| [ExportQuotePrefix](../../aspose.cells/txtsaveoptions/exportquoteprefix/) { get; set; } | Indica se il segno di apice singolo deve essere esportato come parte del valore di una cella quando [`QuotePrefix`](../style/quoteprefix/) è true per essa. Il valore predefinito è false. |
| [FormatStrategy](../../aspose.cells/txtsaveoptions/formatstrategy/) { get; set; } | Ottiene e imposta la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [KeepSeparatorsForBlankRow](../../aspose.cells/txtsaveoptions/keepseparatorsforblankrow/) { get; set; } | Indica se i separatori devono essere emessi per una riga vuota. Il valore predefinito è false, quindi per impostazione predefinita il contenuto della riga vuota sarà vuoto. |
| [LightCellsDataProvider](../../aspose.cells/txtsaveoptions/lightcellsdataprovider/) { get; set; } | Il provider di dati per salvare la cartella di lavoro in modalità leggera. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [QuoteType](../../aspose.cells/txtsaveoptions/quotetype/) { get; set; } | Ottiene o imposta come citare i valori nel file di testo esportato. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [Separator](../../aspose.cells/txtsaveoptions/separator/) { get; set; } | Ottiene e imposta il delimitatore di caratteri del file di testo. |
| [SeparatorString](../../aspose.cells/txtsaveoptions/separatorstring/) { get; set; } | Ottiene e imposta un valore stringa come separatore. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [TrimLeadingBlankRowAndColumn](../../aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/) { get; set; } | Indica se le righe e le colonne vuote iniziali devono essere eliminate come fa MS Excel. Il valore predefinito è true. |
| [TrimTailingBlankCells](../../aspose.cells/txtsaveoptions/trimtailingblankcells/) { get; set; } | Indica se le celle vuote finali in una riga devono essere eliminate. Il valore predefinito è false. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare le impostazioni di smart art. Il valore predefinito è false. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta la callback di avviso.(Ereditato da [`SaveOptions`](../saveoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class TxtSaveOptionsDemo
    {
        public static void TxtSaveOptionsExample()
        {
            // Crea una cartella di lavoro con alcuni dati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Smith");
            worksheet.Cells["B3"].PutValue(25);

            // Crea un oggetto TxtSaveOptions e imposta le proprietà
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                SeparatorString = ",",
                Encoding = Encoding.UTF8,
                AlwaysQuoted = false,
                QuoteType = TxtValueQuoteType.Normal,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                TrimLeadingBlankRowAndColumn = true,
                TrimTailingBlankCells = false,
                KeepSeparatorsForBlankRow = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                ExportQuotePrefix = false,
                ExportAllSheets = false,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Salva la cartella di lavoro come file di testo con le opzioni specificate
            workbook.Save("TxtSaveOptionsExample.txt", saveOptions);

            Console.WriteLine("Workbook saved successfully with TxtSaveOptions.");
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


