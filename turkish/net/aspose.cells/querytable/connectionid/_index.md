---
title: "QueryTable.ConnectionId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "QueryTable özelliği. Sorgu tablosunun bağlantı kimliğini alır"
type: docs
url: /tr/net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

Sorgu tablosunun bağlantı kimliğini alır.

```csharp
public int ConnectionId { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir sorgu tablosu senaryosunu simüle etmek için örnek veri ekle
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Sample Data");

            try
            {
                // Çalışma sayfasında herhangi bir sorgu tablosu olup olmadığını kontrol et
                if (worksheet.QueryTables.Count > 0)
                {
                    // İlk sorgu tablosunu al
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // ConnectionId özelliği değerini göster (yalnızca okunabilir)
                    Console.WriteLine("Query Table ConnectionId: " + queryTable.ConnectionId);

                    // Bağlam için diğer ilgili özellikleri göster
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("External Connection: " +
                        (queryTable.ExternalConnection != null ? queryTable.ExternalConnection.Name : "None"));
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


