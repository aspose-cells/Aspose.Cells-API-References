---
title: "QueryTable.ExternalConnection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "QueryTable özelliği. İlgili dış bağlantıyı alır"
type: docs
url: /tr/net/aspose.cells/querytable/externalconnection/
---
## QueryTable.ExternalConnection property

İlgili dış bağlantıyı alır.

```csharp
public ExternalConnection ExternalConnection { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class QueryTablePropertyExternalConnectionDemo
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

                    // ExternalConnection özelliğine eriş (yalnızca okunabilir)
                    ExternalConnection externalConnection = queryTable.ExternalConnection;

                    // Dış bağlantı hakkında bilgileri göster
                    if (externalConnection != null)
                    {
                        Console.WriteLine("External Connection ID: " + externalConnection.Id);
                        Console.WriteLine("External Connection Name: " + externalConnection.Name);
                        Console.WriteLine("External Connection Type: " + externalConnection.ClassType);
                        Console.WriteLine("Connection String: " + externalConnection.ConnectionString);
                        Console.WriteLine("Refresh on Load: " + externalConnection.RefreshOnLoad);
                    }
                    else
                    {
                        Console.WriteLine("No external connection associated with this query table.");
                    }

                    // Bağlam için diğer sorgu tablosu özelliklerini göster
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


