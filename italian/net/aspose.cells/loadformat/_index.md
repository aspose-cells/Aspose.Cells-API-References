---
title: "Enum LoadFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.LoadFormat enum. Rappresenta il formato di caricamento del file"
type: docs
url: /it/net/aspose.cells/loadformat/
---
## LoadFormat enumeration

Rappresenta il formato di caricamento del file.

```csharp
public enum LoadFormat
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Auto | `0` | Rappresenta il riconoscimento automatico del formato. |
| Csv | `1` | File di testo CSV (valori separati da virgola). |
| CSV | `1` | File di testo CSV (valori separati da virgola). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Csv. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| Xlsx | `6` | Rappresenta un workbook o modello Office Open XML spreadsheetML, con o senza macro. |
| Tsv | `11` | File di testo TSV (valori separati da tabulazione). |
| TSV | `11` | File di testo TSV (valori separati da tabulazione). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Tsv. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| TabDelimited | `11` | Rappresenta un file di testo delimitato da tabulazione, uguale a Tsv. |
| Html | `12` | Rappresenta un file HTML. |
| MHtml | `13` | Rappresenta un file MHTML. |
| Ods | `14` | File Open Document Sheet (ODS). |
| ODS | `14` | File Open Document Sheet (ODS). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Ods. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| Excel97To2003 | `5` | Rappresenta un file Excel97-2003 xls. |
| SpreadsheetML | `15` | Rappresenta un file Excel 2003 xml. |
| Xlsb | `16` | Rappresenta un file xlsb. |
| Ots | `31` | File Open Document Template Sheet (OTS). |
| Numbers | `56` | Rappresenta un file Numbers. |
| Fods | `59` | Rappresenta il formato di file OpenDocument Flat XML Spreadsheet (.fods). |
| FODS | `59` | Rappresenta il formato di file OpenDocument Flat XML Spreadsheet (.fods). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Fods. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| Sxc | `60` | Rappresenta il formato di file StarOffice Calc Spreadsheet (.sxc). |
| SXC | `60` | Rappresenta il formato di file StarOffice Calc Spreadsheet (.sxc). NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Sxc. Questa proprietà sarà rimossa 6 mesi dopo, a partire da aprile 2021. Aspose si scusa per qualsiasi inconveniente tu possa aver sperimentato. |
| Xml | `51` | Rappresenta un file XML semplice. |
| Epub | `52` | Rappresenta un file EPUB. |
| Azw3 | `53` | Rappresenta un file AZW3. |
| Chm | `54` | Rappresenta un file CHM. |
| Markdown | `55` | Rappresenta un file Markdown. |
| Unknown | `255` | Rappresenta un formato non riconosciuto, impossibile da caricare. |
| Image | `254` | Immagine |
| Json | `513` | Json |
| Dif | `30` | Formato di scambio dati. |
| Dbf | `515` | File dati Xbase |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFormatDemo
    {
        public static void LoadFormatExample()
        {
            // Carica un file Excel in diversi formati usando Aspose.Cells
            string[] filePaths = {
                "LoadFormatDemo_original.xlsx",
                "LoadFormatDemo_original.xls",
                "LoadFormatDemo_original.csv",
                "LoadFormatDemo_original.json"
            };

            foreach (var filePath in filePaths)
            {
                // Determina il formato di caricamento in base all'estensione del file
                LoadFormat loadFormat = GetLoadFormat(filePath);

                // Crea LoadOptions con il LoadFormat determinato
                LoadOptions loadOptions = new LoadOptions(loadFormat);

                // Carica la cartella di lavoro con le opzioni di caricamento specificate
                Workbook workbook = new Workbook(filePath, loadOptions);

                // Esegui alcune operazioni sulla cartella di lavoro
                Console.WriteLine($"Loaded file: {filePath}");
                Console.WriteLine($"Number of sheets: {workbook.Worksheets.Count}");

                // Salva la cartella di lavoro in un nuovo file
                string outputFilePath = $"output_{System.IO.Path.GetFileName(filePath)}";
                workbook.Save(outputFilePath);
                Console.WriteLine($"Saved file as: {outputFilePath}");
            }
        }

        private static LoadFormat GetLoadFormat(string filePath)
        {
            string extension = System.IO.Path.GetExtension(filePath).ToLower();
            switch (extension)
            {
                case ".xlsx":
                    return LoadFormat.Xlsx;
                case ".xls":
                    return LoadFormat.Excel97To2003;
                case ".csv":
                    return LoadFormat.Csv;
                case ".json":
                    return LoadFormat.Json;
                default:
                    return LoadFormat.Auto;
            }
        }
    }

}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


