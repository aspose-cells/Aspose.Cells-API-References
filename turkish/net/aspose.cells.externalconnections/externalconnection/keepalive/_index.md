---
title: "ExternalConnection.KeepAlive"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bağlantının açık tutulması için elektronik tablo uygulamasının çaba göstermesi gerektiğinde doğru (True). Yanlış (false) olduğunda uygulama, bilgiyi aldıktan sonra bağlantıyı kapatmalıdır."
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/keepalive/
---
## ExternalConnection.KeepAlive property

Bağlantının açık tutulması için elektronik tablo uygulamasının çaba göstermesi gerektiğinde true. False olduğunda, uygulama bilgiyi aldıktan sonra bağlantıyı kapatmalıdır.

```csharp
public bool KeepAlive { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyKeepAliveDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya erişin (var olduğunu varsayarak)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mevcut KeepAlive değerini görüntüle
                Console.WriteLine("Initial KeepAlive value: " + connection.KeepAlive);
                
                // KeepAlive değerini değiştir (okunabilir-yazılabilir olduğu için)
                connection.KeepAlive = !connection.KeepAlive;
                Console.WriteLine("Updated KeepAlive value: " + connection.KeepAlive);
                
                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("KeepAliveDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


