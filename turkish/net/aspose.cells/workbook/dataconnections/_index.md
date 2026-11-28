---
title: "Workbook.DataConnections"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. ExternalConnection koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

[`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/) koleksiyonunu alır.

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookPropertyDataConnectionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Örnek bir çalışma sayfası oluşturun
            Worksheet worksheet = workbook.Worksheets[0];

            // Örneği anlamlı kılmak için bazı veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // DataConnections özelliğine erişin
                var dataConnections = workbook.DataConnections;

                // Özelliğin mevcut değerini göster (okuma işlemi)
                Console.WriteLine("DataConnections count: " + dataConnections.Count);

                // Mevcut bağlantılar varsa, üzerinden döngü yapın
                for (int i = 0; i < dataConnections.Count; i++)
                {
                    var connection = dataConnections[i];
                    Console.WriteLine($"Connection {i + 1}: {connection.Name}");
                }

                // Özelliğin davranışı nasıl etkilediğini göster
                Console.WriteLine("DataConnections has been demonstrated");

                // Sonucu kaydet
                workbook.Save("DataConnectionsDemo.xlsx");
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

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


