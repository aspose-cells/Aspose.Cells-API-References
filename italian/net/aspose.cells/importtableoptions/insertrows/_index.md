---
title: "ImportTableOptions.InsertRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Indica se devono essere aggiunte nuove righe per l'importazione dei record di dati"
type: docs
url: /it/net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

Indica se devono essere aggiunte nuove righe per l'importazione dei record di dati.

```csharp
public bool InsertRows { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyInsertRowsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea una tabella di dati di esempio
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            dataTable.Rows.Add(1, "Laptop", 999.99);
            dataTable.Rows.Add(2, "Monitor", 249.99);
            dataTable.Rows.Add(3, "Keyboard", 49.99);

            // Aggiungi i dati esistenti al foglio di lavoro (verranno spostati verso il basso dall'inserimento)
            cells["A1"].PutValue("Existing Data");
            cells["A2"].PutValue(100);

            // Imposta le opzioni di importazione con InsertRows = true
            ImportTableOptions options = new ImportTableOptions();
            options.InsertRows = true; // This will insert new rows instead of overwriting
            options.IsFieldNameShown = true;

            // Importa i dati a partire dalla riga 1 (inserirà righe sotto i dati esistenti)
            cells.ImportData(dataTable, 1, 0, options);

            // Salva la cartella di lavoro
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


