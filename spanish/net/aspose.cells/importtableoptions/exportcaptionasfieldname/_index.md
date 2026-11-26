---
title: "ImportTableOptions.ExportCaptionAsFieldName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImportTableOptions. Indica si se exporta el título como nombre de campo"
type: docs
url: /es/net/aspose.cells/importtableoptions/exportcaptionasfieldname/
---
## ImportTableOptions.ExportCaptionAsFieldName property

Indica si se exporta el título como nombre de campo

```csharp
public bool ExportCaptionAsFieldName { get; set; }
```

### Observaciones

Solo funciona para DataTable.

### Ejemplos

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
            // Crear datos de ejemplo
            List<Transaction> transactions = new List<Transaction>
            {
                new Transaction { orderId = "w101", paymentType = "card", orderType = "bur" },
                new Transaction { orderId = "w102", paymentType = "cash", orderType = "piz" },
                new Transaction { orderId = "w103", paymentType = "card", orderType = "sal" }
            };

            // Crear libro de trabajo e importar datos con ExportCaptionAsFieldName
            Workbook workbook = new Workbook();
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.ExportCaptionAsFieldName = true;
            workbook.Worksheets[0].Cells.ImportCustomObjects(transactions, 0, 0, importOptions);

            // Exportar datos de nuevo para verificar
            ExportTableOptions exportOptions = new ExportTableOptions();
            List<Transaction> exportedData = workbook.Worksheets[0].Cells.ExportList<Transaction>(0, 0, 5, 10, exportOptions);

            // Mostrar verificación
            Console.WriteLine($"Exported count: {exportedData.Count}");
            Console.WriteLine($"First payment type: {exportedData[0].paymentType}");
        }
    }
}
```

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


