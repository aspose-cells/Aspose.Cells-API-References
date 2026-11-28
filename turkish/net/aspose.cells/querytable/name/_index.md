---
title: "QueryTable.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "QueryTable özelliği. Sorgu tablosunun adını alır"
type: docs
url: /tr/net/aspose.cells/querytable/name/
---
## QueryTable.Name property

Sorgu tablosunun adını alır.

```csharp
public string Name { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Sorgu tablosunu simüle etmek için örnek veri ekle
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Çalışma sayfasında herhangi bir sorgu tablosu olup olmadığını kontrol et
                if (worksheet.QueryTables.Count > 0)
                {
                    // İlk sorgu tablosunu al
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Name özelliği değerini göster (yalnızca okunabilir işlem)
                    Console.WriteLine("Query Table Name: " + queryTable.Name);

                    // Bağlam için diğer yalnızca okunabilir özellikleri göster
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("QueryTableNameDemo.xlsx");
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


