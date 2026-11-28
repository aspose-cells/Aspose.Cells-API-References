---
title: "Worksheet.QueryTables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Çalışma sayfasındaki QueryTableCollection'ı alır"
type: docs
url: /tr/net/aspose.cells/worksheet/querytables/
---
## Worksheet.QueryTables property

Çalışma sayfasındaki [`QueryTableCollection`](../../querytablecollection/) öğesini alır.

```csharp
public QueryTableCollection QueryTables { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyQueryTablesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // İlk sorgu tablosunu al (çünkü yeni ekleyemiyoruz doğrudan)
            // Not: QueryTables koleksiyonu bu API sürümünde yalnızca okunabilir
            if (worksheet.QueryTables.Count > 0)
            {
                QueryTable queryTable = worksheet.QueryTables[0];
                
                // Sorgu tablosu bilgilerini göster
                Console.WriteLine("Query Table Name: " + queryTable.Name);
                Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                Console.WriteLine("Number of Query Tables: " + worksheet.QueryTables.Count);
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("QueryTableDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


