---
title: "Classe JsonSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.JsonSaveOptions classe. Rappresenta le opzioni per salvare la cartella di lavoro come file JSON"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/
---
## JsonSaveOptions class

Rappresenta le opzioni di salvataggio della cartella di lavoro come file JSON.

```csharp
public class JsonSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [JsonSaveOptions](jsonsaveoptions/)() | Crea opzioni per salvare il file JSON. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlwaysExportAsJsonObject](../../aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/) { get; set; } | Indica se esportare sempre Excel in JSON come oggetto, anche quando c'è solo un foglio di lavoro nel file. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi il workbook vuoto dopo aver salvato il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ExportArea](../../aspose.cells/jsonsaveoptions/exportarea/) { get; set; } | Ottiene o imposta l'intervallo di esportazione. |
| [ExportAsString](../../aspose.cells/jsonsaveoptions/exportasstring/) { get; set; } | Esporta il valore stringa delle celle in JSON. |
| [ExportEmptyCells](../../aspose.cells/jsonsaveoptions/exportemptycells/) { get; set; } | Indica se esportare le celle vuote come null. |
| [ExportHyperlinkType](../../aspose.cells/jsonsaveoptions/exporthyperlinktype/) { get; set; } | Rappresenta il tipo di esportazione dei collegamenti ipertestuali in JSON. |
| [ExportNestedStructure](../../aspose.cells/jsonsaveoptions/exportnestedstructure/) { get; set; } | Esportato come struttura JSON gerarchica padre-figlio. |
| [ExportStylePool](../../aspose.cells/jsonsaveoptions/exportstylepool/) { get; set; } | Indica se esportare gli stili collettivamente o individualmente per ogni cella. |
| [HasHeaderRow](../../aspose.cells/jsonsaveoptions/hasheaderrow/) { get; set; } | Indica se l'intervallo contiene la riga di intestazione. |
| [Indent](../../aspose.cells/jsonsaveoptions/indent/) { get; set; } | Indica l'indentazione. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [Schemas](../../aspose.cells/jsonsaveoptions/schemas/) { get; set; } | Lo schema JSON originale di ogni foglio di lavoro. |
| [SheetIndexes](../../aspose.cells/jsonsaveoptions/sheetindexes/) { get; set; } | Rappresenta gli indici dei fogli esportati. |
| [SkipEmptyRows](../../aspose.cells/jsonsaveoptions/skipemptyrows/) { get; set; } | Indica se saltare le righe vuote. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ToExcelStruct](../../aspose.cells/jsonsaveoptions/toexcelstruct/) { get; set; } | Indica se convertire in una struttura JSON del file Excel. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare le impostazioni di smart art. Il valore predefinito è false. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta la callback di avviso.(Ereditato da [`SaveOptions`](../saveoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Json;
    using System;

    public class JsonSaveOptionsDemo
    {
        public static void JsonSaveOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci alcuni dati nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Crea un'istanza di JsonSaveOptions
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                ExportHyperlinkType = JsonExportHyperlinkType.DisplayString,
                SkipEmptyRows = true,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ExportAsString = true,
                Indent = "  ",
                ExportNestedStructure = false,
                ExportEmptyCells = false,
                AlwaysExportAsJsonObject = false,
                ToExcelStruct = false,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Salva la cartella di lavoro come file JSON
            workbook.Save("JsonSaveOptionsExample.json", saveOptions);

            return;
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


