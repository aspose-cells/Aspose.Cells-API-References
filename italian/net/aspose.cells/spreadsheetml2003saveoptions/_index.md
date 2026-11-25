---
title: "Classe SpreadsheetML2003SaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.SpreadsheetML2003SaveOptions. Rappresenta le opzioni per salvare un file spreadml Excel 2003"
type: docs
url: /it/net/aspose.cells/spreadsheetml2003saveoptions/
---
## SpreadsheetML2003SaveOptions class

Rappresenta le opzioni per salvare il file Excel 2003 spreadml.

```csharp
public class SpreadsheetML2003SaveOptions : SaveOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SpreadsheetML2003SaveOptions](spreadsheetml2003saveoptions/#constructor)() | Crea le opzioni per salvare un file spreadml Excel 2003. |
| [SpreadsheetML2003SaveOptions](spreadsheetml2003saveoptions/#constructor_1)(SaveFormat) | (**Obsoleto.**) Crea le opzioni per salvare un file spreadml Excel 2003. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi il workbook vuoto dopo aver salvato il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento durante il salvataggio come file .xls. Il valore predefinito è true. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ExportColumnIndexOfCell](../../aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/) { get; set; } | Il valore predefinito è false, significa che l'indice della colonna verrà ignorato se la cella è contigua alla cella precedente. |
| [IsIndentedFormatting](../../aspose.cells/spreadsheetml2003saveoptions/isindentedformatting/) { get; set; } | Fa sì che gli elementi figli siano indentati. |
| [LimitAsXls](../../aspose.cells/spreadsheetml2003saveoptions/limitasxls/) { get; set; } | Limite per xls, l'indice massimo di riga è 65535 e l'indice massimo di colonna è 255. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare le impostazioni di smart art. Il valore predefinito è false. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. (Ereditato da [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta la callback di avviso.(Ereditato da [`SaveOptions`](../saveoptions/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SpreadsheetML2003SaveOptionsDemo
    {
        public static void SpreadsheetML2003SaveOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci alcuni dati nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["B2"].PutValue(456);

            // Crea un'istanza di SpreadsheetML2003SaveOptions
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();

            // Imposta le proprietà
            saveOptions.IsIndentedFormatting = true;
            saveOptions.LimitAsXls = false;
            saveOptions.ExportColumnIndexOfCell = true;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = @"C:\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = true;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = true;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Salva la cartella di lavoro con le opzioni di salvataggio specificate
            workbook.Save("SpreadsheetML2003Example.xml", saveOptions);

            return;
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


