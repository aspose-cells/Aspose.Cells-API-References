---
title: "ExportTableOptions.ExportAsString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExportTableOptions. Esporta il valore stringa delle celle nella DataTable"
type: docs
url: /it/net/aspose.cells/exporttableoptions/exportasstring/
---
## ExportTableOptions.ExportAsString property

Esporta il valore stringa delle celle nella DataTable.

```csharp
public bool ExportAsString { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con tipi misti
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue(123.45);
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("TextValue");

            // Crea opzioni di esportazione con ExportAsString impostato su true
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                ExportAsString = true // This forces all values to be exported as strings
            };

            // Esporta i dati in DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Visualizza i tipi di dati esportati
            Console.WriteLine("Data exported with ExportAsString=true:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }

            // Ora esporta con ExportAsString=false
            exportOptions.ExportAsString = false;
            DataTable dataTable2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            Console.WriteLine("\nData exported with ExportAsString=false:");
            foreach (DataRow row in dataTable2.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


