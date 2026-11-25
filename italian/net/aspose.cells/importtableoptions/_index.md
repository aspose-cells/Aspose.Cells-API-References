---
title: "Classe ImportTableOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ImportTableOptions. Rappresenta le opzioni per l'importazione dei dati nelle celle"
type: docs
url: /it/net/aspose.cells/importtableoptions/
---
## ImportTableOptions class

Rappresenta le opzioni di importazione dei dati nelle celle.

```csharp
public class ImportTableOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ImportTableOptions](importtableoptions/)() | Crea le opzioni di importazione predefinite. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CheckMergedCells](../../aspose.cells/importtableoptions/checkmergedcells/) { get; set; } | Indica se controllare le celle unite. |
| [ColumnIndexes](../../aspose.cells/importtableoptions/columnindexes/) { get; set; } | Ottiene o imposta le colonne (indice 0) da importare dalla fonte dati. null indica che tutte le colonne devono essere importate. |
| [ConvertGridStyle](../../aspose.cells/importtableoptions/convertgridstyle/) { get; set; } | Indica se applicare lo stile della visualizzazione a griglia alle celle. |
| [ConvertNumericData](../../aspose.cells/importtableoptions/convertnumericdata/) { get; set; } | Ottiene o imposta un valore che indica se la stringa deve essere convertita in valore numerico o data. |
| [DateFormat](../../aspose.cells/importtableoptions/dateformat/) { get; set; } | Ottiene o imposta la stringa di formato data per le celle con valori datetime importati. |
| [DefaultValues](../../aspose.cells/importtableoptions/defaultvalues/) { get; set; } | Il valore predefinito per il valore nella tabella è null. |
| [ExportCaptionAsFieldName](../../aspose.cells/importtableoptions/exportcaptionasfieldname/) { get; set; } | Indica se esportare la didascalia come nome campo |
| [InsertRows](../../aspose.cells/importtableoptions/insertrows/) { get; set; } | Indica se devono essere aggiunte nuove righe per l'importazione dei record di dati. |
| [IsFieldNameShown](../../aspose.cells/importtableoptions/isfieldnameshown/) { get; set; } | Indica se il nome campo deve essere importato. |
| [IsFormulas](../../aspose.cells/importtableoptions/isformulas/) { get; set; } | Indica se i dati sono formule. |
| [IsHtmlString](../../aspose.cells/importtableoptions/ishtmlstring/) { get; set; } | Indica se il valore contiene tag HTML. |
| [NumberFormats](../../aspose.cells/importtableoptions/numberformats/) { get; set; } | Ottiene o imposta i formati numerici |
| [ShiftFirstRowDown](../../aspose.cells/importtableoptions/shiftfirstrowdown/) { get; set; } | Indica se spostare verso il basso la prima riga durante l'inserimento di righe. |
| [Styles](../../aspose.cells/importtableoptions/styles/) { get; set; } | Ottiene e imposta gli stili per ogni colonna della tabella. |
| [TotalColumns](../../aspose.cells/importtableoptions/totalcolumns/) { get; set; } | Ottiene o imposta il conteggio totale delle colonne da importare dalla fonte dati. -1 indica tutte le righe della fonte dati fornita. |
| [TotalRows](../../aspose.cells/importtableoptions/totalrows/) { get; set; } | Ottiene o imposta il conteggio totale delle righe da importare dalla fonte dati. -1 indica tutte le righe della fonte dati fornita. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsDemo
    {
        public static void ImportTableOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una DataTable da importare
            DataTable dataTable = new DataTable("SampleData");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Date", typeof(DateTime));
            dataTable.Rows.Add(1, "John Doe", DateTime.Now);
            dataTable.Rows.Add(2, "Jane Smith", DateTime.Now.AddDays(1));

            // Crea un'istanza di ImportTableOptions
            ImportTableOptions importOptions = new ImportTableOptions
            {
                ConvertGridStyle = true,
                ConvertNumericData = true,
                InsertRows = true,
                ShiftFirstRowDown = false,
                IsFieldNameShown = true,
                ExportCaptionAsFieldName = false,
                DateFormat = "yyyy-MM-dd",
                TotalRows = -1, // Import all rows
                TotalColumns = -1, // Import all columns
                IsHtmlString = false,
                CheckMergedCells = false
            };

            // Importa la DataTable nel foglio di lavoro
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Salva la cartella di lavoro
            workbook.Save("ImportTableOptionsExample.xlsx");
            workbook.Save("ImportTableOptionsExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


