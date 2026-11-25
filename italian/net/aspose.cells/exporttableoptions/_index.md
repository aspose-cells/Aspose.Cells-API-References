---
title: "Classe ExportTableOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ExportTableOptions. Rappresenta tutte le opzioni di esportazione della tabella"
type: docs
url: /it/net/aspose.cells/exporttableoptions/
---
## ExportTableOptions class

Rappresenta tutte le opzioni di esportazione della tabella.

```csharp
public class ExportTableOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ExportTableOptions](exporttableoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AllowDBNull](../../aspose.cells/exporttableoptions/allowdbnull/) { get; set; } | Questo valore indica se i DBNull sono consentiti in questa tabella. |
| [CheckMixedValueType](../../aspose.cells/exporttableoptions/checkmixedvaluetype/) { get; set; } | False, Aspose.Cells imposterà il tipo della DataColumn in base al tipo di valore della prima riga per motivi di prestazioni. True, Aspose.Cells verificherà se il tipo di valore nella colonna è misto prima di impostare il tipo della DataColumn e, se i tipi di valore sono misti, il tipo della DataColumn sarà string. |
| [DataTable](../../aspose.cells/exporttableoptions/datatable/) { get; set; } | Ottiene e imposta la DataTable a cui è assegnato il tipo di dati delle colonne. |
| [ExportAsHtmlString](../../aspose.cells/exporttableoptions/exportashtmlstring/) { get; set; } | Esporta il valore stringa HTML delle celle nella DataTable. |
| [ExportAsString](../../aspose.cells/exporttableoptions/exportasstring/) { get; set; } | Esporta il valore stringa delle celle nella DataTable. |
| [ExportColumnName](../../aspose.cells/exporttableoptions/exportcolumnname/) { get; set; } | Indica se i dati nella prima riga vengono esportati nel nome della colonna della DataTable. Il valore predefinito è false. |
| [FormatStrategy](../../aspose.cells/exporttableoptions/formatstrategy/) { get; set; } | Ottiene e imposta la strategia di formattazione quando si esporta il valore come valore stringa. |
| [Indexes](../../aspose.cells/exporttableoptions/indexes/) { get; set; } | Gli indici delle colonne/righe che devono essere esportati. |
| [IsVertical](../../aspose.cells/exporttableoptions/isvertical/) { get; set; } | True se una riga nel file Workbook rappresenta una riga nella DataTable. False se una colonna nel file Workbook rappresenta una riga nella DataTable. |
| [PlotVisibleCells](../../aspose.cells/exporttableoptions/plotvisiblecells/) { get; set; } | Esporta solo le celle visibili. |
| [PlotVisibleColumns](../../aspose.cells/exporttableoptions/plotvisiblecolumns/) { get; set; } | Esporta solo le colonne visibili. |
| [PlotVisibleRows](../../aspose.cells/exporttableoptions/plotvisiblerows/) { get; set; } | Esporta solo le righe visibili. |
| [RenameStrategy](../../aspose.cells/exporttableoptions/renamestrategy/) { get; set; } | Strategia per i nomi duplicati delle colonne. |
| [SkipErrorValue](../../aspose.cells/exporttableoptions/skiperrorvalue/) { get; set; } | Indica se ignorare i valori non validi per la colonna. Ad esempio, se il tipo della colonna è decimal, il valore è maggiore di decimal.MaxValue e questa proprietà è true, non verrà sollevata nuovamente un'eccezione. Il valore predefinito è false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [PreprocessExportedValue](../../aspose.cells/exporttableoptions/preprocessexportedvalue/)(int, int, CellValue) | Preelabora il valore della cella corrente da esportare. |

### Osservazioni

Se ci sono requisiti speciali per l'esportazione, come ignorare i valori di errore, l'utente può estendere questa classe per sovrascrivere le API corrispondenti e raggiungere l'obiettivo.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ExportTableOptionsDemo
    {
        public static void ExportTableOptionsExample()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio al foglio di lavoro
            worksheet.Cells[0, 0].PutValue("Name");
            worksheet.Cells[0, 1].PutValue("Age");
            worksheet.Cells[1, 0].PutValue("John");
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue("Jane");
            worksheet.Cells[2, 1].PutValue(25);

            // Crea un'istanza di ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                SkipErrorValue = true,
                PlotVisibleCells = true,
                PlotVisibleRows = true,
                PlotVisibleColumns = true,
                ExportAsString = false,
                ExportAsHtmlString = false,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                CheckMixedValueType = true,
                AllowDBNull = true,
                IsVertical = true,
                RenameStrategy = RenameStrategy.Digit
            };

            // Esporta i dati dal foglio di lavoro a una DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Visualizza i dati esportati
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Salva la cartella di lavoro
            workbook.Save("ExportTableOptionsExample.xlsx");
            workbook.Save("ExportTableOptionsExample.pdf");
        }
    }

}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


