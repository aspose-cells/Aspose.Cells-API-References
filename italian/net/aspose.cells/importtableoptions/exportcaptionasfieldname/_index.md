---
title: "ImportTableOptions.ExportCaptionAsFieldName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImportTableOptions. Indica se esportare la didascalia come nome campo"
type: docs
url: /it/net/aspose.cells/importtableoptions/exportcaptionasfieldname/
---
## ImportTableOptions.ExportCaptionAsFieldName property

Indica se esportare la didascalia come nome campo

```csharp
public bool ExportCaptionAsFieldName { get; set; }
```

### Osservazioni

Funziona solo per DataTable.

### Esempi

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyExportCaptionAsFieldNameDemo
    {
        public class Transaction
        {
            public string orderId { get; set; }
            public string paymentType { get; set; }
            public string orderType { get; set; }
        }

        public static void Run()
        {
            // Crea dati di esempio
            List<Transaction> transactions = new List<Transaction>
            {
                new Transaction { orderId = "w101", paymentType = "card", orderType = "bur" },
                new Transaction { orderId = "w102", paymentType = "cash", orderType = "piz" },
                new Transaction { orderId = "w103", paymentType = "card", orderType = "sal" }
            };

            // Crea una cartella di lavoro e importa dati con ExportCaptionAsFieldName
            Workbook workbook = new Workbook();
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.ExportCaptionAsFieldName = true;
            workbook.Worksheets[0].Cells.ImportCustomObjects(transactions, 0, 0, importOptions);

            // Esporta nuovamente i dati per verificare
            ExportTableOptions exportOptions = new ExportTableOptions();
            List<Transaction> exportedData = workbook.Worksheets[0].Cells.ExportList<Transaction>(0, 0, 5, 10, exportOptions);

            // Verifica dell'output
            Console.WriteLine($"Exported count: {exportedData.Count}");
            Console.WriteLine($"First payment type: {exportedData[0].paymentType}");
        }
    }
}
```

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


