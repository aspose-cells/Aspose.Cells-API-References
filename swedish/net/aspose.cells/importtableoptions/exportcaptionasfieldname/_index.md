---
title: "ImportTableOptions.ExportCaptionAsFieldName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions egenskap. Anger om rubrik exporteras som fältnamn"
type: docs
url: /sv/net/aspose.cells/importtableoptions/exportcaptionasfieldname/
---
## ImportTableOptions.ExportCaptionAsFieldName property

Anger om rubriken ska exporteras som fältnamn

```csharp
public bool ExportCaptionAsFieldName { get; set; }
```

### Anmärkningar

Fungerar endast för DataTable.

### Exempel

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
            // Skapa exempeldata
            List<Transaction> transactions = new List<Transaction>
            {
                new Transaction { orderId = "w101", paymentType = "card", orderType = "bur" },
                new Transaction { orderId = "w102", paymentType = "cash", orderType = "piz" },
                new Transaction { orderId = "w103", paymentType = "card", orderType = "sal" }
            };

            // Skapa arbetsbok och importera data med ExportCaptionAsFieldName
            Workbook workbook = new Workbook();
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.ExportCaptionAsFieldName = true;
            workbook.Worksheets[0].Cells.ImportCustomObjects(transactions, 0, 0, importOptions);

            // Exportera data igen för att verifiera
            ExportTableOptions exportOptions = new ExportTableOptions();
            List<Transaction> exportedData = workbook.Worksheets[0].Cells.ExportList<Transaction>(0, 0, 5, 10, exportOptions);

            // Utskriftsverifiering
            Console.WriteLine($"Exported count: {exportedData.Count}");
            Console.WriteLine($"First payment type: {exportedData[0].paymentType}");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


