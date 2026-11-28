---
title: "ExternalConnection.OdcFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bu bağlantının oluşturulduğu dış bağlantı dosyasının tam yolunu belirtir. Bir bağlantı, veri yenileme girişimi sırasında ve reconnectionMethod1 sırasında başarısız olursa, elektronik tablo uygulaması, çalışma kitabına gömülü bağlantı nesnesi yerine dış bağlantı dosyasındaki bilgileri kullanarak tekrar deneyecektir."
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/odcfile/
---
## ExternalConnection.OdcFile property

Bu bağlantının oluşturulduğu harici bağlantı dosyasının tam yolunu belirtir. Veri yenileme girişimi sırasında bir bağlantı başarısız olur ve reconnectionMethod=1 ise, elektronik tablo uygulaması, çalışma kitabına gömülü bağlantı nesnesi yerine harici bağlantı dosyasındaki bilgileri kullanarak yeniden deneyecektir.

```csharp
public string OdcFile { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOdcFileDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya erişin (var olduğunu varsayarak)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mevcut OdcFile değerini göster
                Console.WriteLine("Initial OdcFile value: " + connection.OdcFile);
                
                // Yeni bir OdcFile değeri ayarlayın (okuma-yazma olduğu için)
                connection.OdcFile = @"C:\Connections\ExternalData.odc";
                Console.WriteLine("Updated OdcFile value: " + connection.OdcFile);
                
                // OdcFile değerini temizleyin
                connection.OdcFile = string.Empty;
                Console.WriteLine("Cleared OdcFile value: " + connection.OdcFile);
                
                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("OdcFileDemo.xlsx");
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


