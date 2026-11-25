---
title: "Classe SaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.SaveOptions. Rappresenta tutte le opzioni di salvataggio"
type: docs
url: /it/net/aspose.cells/saveoptions/
---
## SaveOptions class

Rappresenta tutte le opzioni di salvataggio

```csharp
public class SaveOptions
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La cartella per i file temporanei che possono essere usati come cache dei dati. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato. |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Rendi la cartella di lavoro vuota dopo aver salvato il file. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Se true e la directory non esiste, la directory verrà creata automaticamente prima di salvare il file. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica se crittografare le proprietà del documento quando si salva come file .xls. Il valore predefinito è true. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica se unire le aree di formattazione condizionale e convalida prima di salvare il file. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica se memorizzare nella cache gli ultimi dati del grafico. |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ottiene il formato di salvataggio del file. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica se ordinare i nomi definiti esterni prima di salvare il file. |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica se ordinare i nomi definiti prima di salvare il file. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica se aggiornare l'impostazione SmartArt. Il valore predefinito è false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica se convalidare le celle unite prima di salvare il file. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ottiene o imposta il callback di avviso. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassSaveOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Crea opzioni di salvataggio - salva come CSV
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = ',';
            
            // Crea opzioni di caricamento per CSV
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);

            // Risalva la cartella di lavoro utilizzando le opzioni
            Workbook resavedWorkbook = Cells_Type_SaveOptions(workbook, saveOptions, loadOptions);

            // Salva il risultato su file
            resavedWorkbook.Save("output.csv", SaveFormat.Csv);
        }

        public static Workbook Cells_Type_SaveOptions(Workbook wb, SaveOptions optsSave, LoadOptions optsLoad)
        {
            using (MemoryStream ms = new MemoryStream(1048576))
            {
                wb.Save(ms, optsSave);
                ms.Position = 0;
                return new Workbook(ms, optsLoad);
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


