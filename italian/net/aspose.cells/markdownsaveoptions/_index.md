---
title: "Classe MarkdownSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.MarkdownSaveOptions. Rappresenta le opzioni di salvataggio per markdown"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/
---
## MarkdownSaveOptions class

Rappresenta le opzioni di salvataggio per markdown.

```csharp
public class MarkdownSaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [MarkdownSaveOptions](markdownsaveoptions/)() | Crea le opzioni per salvare il documento markdown |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlignColumnPadding](../../aspose.cells/markdownsaveoptions/aligncolumnpadding/) { get; set; } | Indica se l'allineamento delle colonne è abilitato per le tabelle Markdown generate. Quando abilitato, le colonne sono allineate riempiendo il contenuto delle celle con il carattere specificato (tipicamente ' ' per gli spazi). Impostare su '\0' per disabilitare l'allineamento delle colonne (predefinito). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/markdownsaveoptions/calculateformula/) { get; set; } | Indica se calcolare le formule prima di salvare il file markdown. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi il workbook vuoto dopo aver salvato il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/markdownsaveoptions/encoding/) { get; set; } | Ottiene e imposta la codifica predefinita. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ExportHyperlinkAsReference](../../aspose.cells/markdownsaveoptions/exporthyperlinkasreference/) { get; set; } | Indica se esportare i collegamenti ipertestuali usando definizioni di riferimento invece del formato inline. Il valore predefinito è false. |
| [ExportImagesAsBase64](../../aspose.cells/markdownsaveoptions/exportimagesasbase64/) { get; set; } | Specifica se le immagini sono salvate in formato Base64 nel Markdown. Il valore predefinito è true. |
| [FormatStrategy](../../aspose.cells/markdownsaveoptions/formatstrategy/) { get; set; } | Ottiene e imposta la strategia di formattazione quando si esporta il valore della cella come stringa. |
| [ImageOptions](../../aspose.cells/markdownsaveoptions/imageoptions/) { get; } | Ottieni l'oggetto ImageOrPrintOptions prima dell'esportazione |
| [LightCellsDataProvider](../../aspose.cells/markdownsaveoptions/lightcellsdataprovider/) { get; set; } | Il provider di dati per fornire i dati delle celle per salvare la cartella di lavoro in modalità leggera. |
| [LineSeparator](../../aspose.cells/markdownsaveoptions/lineseparator/) { get; set; } | Ottiene e imposta il separatore di riga. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [OfficeMathOutputType](../../aspose.cells/markdownsaveoptions/officemathoutputtype/) { get; set; } | Indica come gli oggetti OfficeMath vengono esportati in Markdown, il valore predefinito è Image. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/markdownsaveoptions/sheetset/) { get; set; } | Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [`Active`](../../aspose.cells.rendering/sheetset/active/). |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SplitTablesByBlankRow](../../aspose.cells/markdownsaveoptions/splittablesbyblankrow/) { get; set; } | Indica se le righe vuote nel foglio di lavoro devono essere trattate come separatori di tabella durante l'esportazione in Markdown. Il valore predefinito è false. |
| [StreamProvider](../../aspose.cells/markdownsaveoptions/streamprovider/) { get; set; } | Ottiene o imposta l'IStreamProvider per l'esportazione degli oggetti. Se `null`, gli oggetti esportati saranno salvati nella stessa directory del file di output. |
| [TableHeaderType](../../aspose.cells/markdownsaveoptions/tableheadertype/) { get; set; } | Ottiene e imposta come impostare l'intestazione della tabella. |
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

    public class MarkdownSaveOptionsDemo
    {
        public static void MarkdownSaveOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Crea un'istanza di MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = "\n",
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Salva la cartella di lavoro come file Markdown
            workbook.Save("MarkdownSaveOptionsExample.md", saveOptions);

            Console.WriteLine("Workbook saved as Markdown file successfully.");
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


