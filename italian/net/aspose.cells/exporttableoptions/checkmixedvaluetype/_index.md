---
title: "ExportTableOptions.CheckMixedValueType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ExportTableOptions proprietà. False Aspose.Cells imposterà il tipo di DataColumns in base al tipo di valore della prima riga per motivi di prestazioni. True Aspose.Cells verificherà se il tipo di valore nella colonna è misto prima di impostare il tipo di DataColumns e, se i tipi di valore sono misti, il tipo di DataColumns sarà string."
type: docs
url: /it/net/aspose.cells/exporttableoptions/checkmixedvaluetype/
---
## ExportTableOptions.CheckMixedValueType property

False, Aspose.Cells imposterà il tipo della DataColumn in base al tipo di valore della prima riga per motivi di prestazioni. True, Aspose.Cells verificherà se il tipo di valore nella colonna è misto prima di impostare il tipo della DataColumn e, se i tipi di valore sono misti, il tipo della DataColumn sarà string.

```csharp
public bool CheckMixedValueType { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyCheckMixedValueTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi intestazioni
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value Date");

            // Aggiungi dati di esempio con tipi misti
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue("2023-01-15");
            worksheet.Cells["A4"].PutValue("3");
            worksheet.Cells["B4"].PutValue(DateTime.Now.AddDays(1));

            // Crea opzioni di esportazione con CheckMixedValueType abilitato
            ExportTableOptions options = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true
            };

            // Esporta i dati in DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 2, options);

            // Visualizza i risultati
            Console.WriteLine("Columns: " + dataTable.Columns.Count);
            Console.WriteLine("Rows: " + dataTable.Rows.Count);
            Console.WriteLine("ID column type: " + dataTable.Columns["ID"].DataType);
            Console.WriteLine("Value Date column type: " + dataTable.Columns["Value Date"].DataType);
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


