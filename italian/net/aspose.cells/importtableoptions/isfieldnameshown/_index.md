---
title: "ImportTableOptions.IsFieldNameShown"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Indica se il nome del campo deve essere importato"
type: docs
url: /it/net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

Indica se il nome campo deve essere importato.

```csharp
public bool IsFieldNameShown { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFieldNameShownDemo
    {
        public static void Run()
        {
            // Crea un DataTable di esempio
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Product");
            
            // Aggiungi dati di esempio
            table.Rows.Add(1, "Laptop");
            table.Rows.Add(2, "Smartphone");
            table.Rows.Add(3, "Tablet");

            // Crea una cartella di lavoro e importa dati con i nomi dei campi mostrati
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;  // Show field names
            options.InsertRows = true;       // Insert new rows
            
            // Importa dati a partire dalla riga 5, colonna 0
            cells.ImportData(table, 5, 0, options);
            
            // Salva la cartella di lavoro
            workbook.Save("ImportDataWithFieldNames.xlsx");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


