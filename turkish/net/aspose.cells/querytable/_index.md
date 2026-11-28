---
title: "Sınıf QueryTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.QueryTable sınıfı. QueryTable bilgilerini temsil eder"
type: docs
url: /tr/net/aspose.cells/querytable/
---
## QueryTable class

QueryTable bilgilerini temsil eder.

```csharp
public class QueryTable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | Nesnenin AdjustColumnWidth özelliğini döndürür veya ayarlar. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | Sorgu tablosunun bağlantı kimliğini alır. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | İlgili dış bağlantıyı alır. |
| [Name](../../aspose.cells/querytable/name/) { get; } | Sorgu tablosunun adını alır. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | Nesnenin PreserveFormatting özelliğini döndürür veya ayarlar. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | Sonucun aralığını alır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassQueryTableDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir sorgu tablosu oluşturmak için örnek veri ekle (dış veri taklit edilerek)
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Çalışma sayfasında herhangi bir sorgu tablosu olup olmadığını kontrol et
            if (worksheet.QueryTables.Count > 0)
            {
                // İlk sorgu tablosunu al
                QueryTable qt = worksheet.QueryTables[0];
                
                // Sorgu tablosu özelliklerini görüntüle
                Console.WriteLine("Query Table Name: " + qt.Name);
                Console.WriteLine("Connection ID: " + qt.ConnectionId);
                Console.WriteLine("Result Range: " + qt.ResultRange.Address);
                Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);
                Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
                
                // Bazı özellikleri değiştir
                qt.PreserveFormatting = true;
                qt.AdjustColumnWidth = false;
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


