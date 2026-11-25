---
title: "ImportTableOptions.TotalRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Ottiene o imposta il conteggio totale delle righe da importare dalla fonte dati. 1 significa tutte le righe della fonte dati specificata"
type: docs
url: /it/net/aspose.cells/importtableoptions/totalrows/
---
## ImportTableOptions.TotalRows property

Ottiene o imposta il conteggio totale delle righe da importare dalla fonte dati. -1 indica tutte le righe della fonte dati fornita.

```csharp
public int TotalRows { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalRowsDemo
    {
        public static void Run()
        {
            // Crea un DataTable di esempio
            DataTable table = new DataTable("TestTable");
            table.Columns.Add("Column1", typeof(string));
            table.Columns.Add("Column2", typeof(int));
            
            // Aggiungi dati di esempio
            table.Rows.Add("Item1", 100);
            table.Rows.Add("Item2", 200);
            table.Rows.Add("Item3", 300);

            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea ImportTableOptions con TotalRows impostato a 2 (importerà solo le prime 2 righe)
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalRows = 2 // Only import 2 rows from the DataTable
            };

            // Importa i dati con le opzioni specificate
            worksheet.Cells.ImportData(table, 0, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("ImportWithTotalRows.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Data imported with TotalRows=2. Only first 2 rows were imported.");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


