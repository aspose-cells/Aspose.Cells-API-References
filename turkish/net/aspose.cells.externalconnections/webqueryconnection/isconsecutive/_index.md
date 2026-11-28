---
title: "WebQueryConnection.IsConsecutive"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Ardışık sınırlayıcıların tek bir sınırlayıcı gibi ele alınması gerekip gerekmediğini gösteren bayrak"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/isconsecutive/
---
## WebQueryConnection.IsConsecutive property

Ardışık ayırıcıların tek bir ayırıcı olarak ele alınması gerektiğini gösteren işaret.

```csharp
public bool IsConsecutive { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsConsecutiveDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk bağlantıya erişerek bir web sorgu bağlantısı oluştur
            // (en az bir bağlantının mevcut olduğu varsayılırsa)
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
            
            try
            {
                // İlk IsConsecutive değerini göster (varsayılan)
                Console.WriteLine("Initial IsConsecutive value: " + connection.IsConsecutive);
                
                // IsConsecutive'i true olarak ayarla
                connection.IsConsecutive = true;
                Console.WriteLine("Updated IsConsecutive value: " + connection.IsConsecutive);
                
                // IsConsecutive'i false olarak geri ayarla
                connection.IsConsecutive = false;
                Console.WriteLine("Final IsConsecutive value: " + connection.IsConsecutive);
                
                // Web sorgu bağlantısı ile çalışma kitabını kaydedin
                workbook.Save("WebQueryConnectionIsConsecutiveDemo.xlsx");
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


