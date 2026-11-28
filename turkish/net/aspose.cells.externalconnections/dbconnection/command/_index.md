---
title: "DBConnection.Command"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DBConnection özelliği. Veri sağlayıcı API'sine dış kaynaktan veri almak için iletilecek veritabanı komutunu içeren dize"
type: docs
url: /tr/net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

Veri sağlayıcı API'sine dış kaynağa etkileşimde bulunarak veri almak için gönderilecek veritabanı komutunu içeren dize.

```csharp
public override string Command { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Harici bağlantıların koleksiyonuna erişin
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Koleksiyondaki ilk DBConnection'ı bulun (varsa)
                DBConnection dbConn = null;
                foreach (ExternalConnection conn in connections)
                {
                    if (conn is DBConnection dbConnection)
                    {
                        dbConn = dbConnection;
                        break;
                    }
                }

                if (dbConn == null)
                {
                    Console.WriteLine("No DBConnection objects found in the workbook.");
                }
                else
                {
                    // Geçerli Command değerini göster (okuma işlemi)
                    Console.WriteLine("Current Command: " + dbConn.Command);

                    // Command ayarlamayı göster (okuma‑yazma özelliği)
                    dbConn.Command = "SELECT * FROM Customers";
                    Console.WriteLine("Updated Command: " + dbConn.Command);
                }

                // Çalışma kitabını kaydedin
                workbook.Save("CommandDemo.xlsx");
                Console.WriteLine("Workbook saved as CommandDemo.xlsx");
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

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


