---
title: "ExternalConnection.OnlyUseConnectionFile"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bağlantı yenilendiğinde, elektronik tablo uygulamasının odcFile özniteliğiyle belirtilen dış bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanıp kullanmayacağını gösterir. Yanlış ise, elektronik tablo uygulaması reconnectionMethod özniteliğiyle belirtilen prosedürü izlemelidir."
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/
---
## ExternalConnection.OnlyUseConnectionFile property

Bağlantı yenilendiğinde elektronik tablo uygulamasının, odcFile özniteliğiyle belirtilen harici bağlantı dosyasındaki bağlantı bilgilerini her zaman ve yalnızca kullanıp kullanmayacağını gösterir. False ise, uygulama reconnectionMethod özniteliğiyle belirtilen prosedürü izlemelidir.

```csharp
public bool OnlyUseConnectionFile { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOnlyUseConnectionFileDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya erişin (var olduğunu varsayarak)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mevcut OnlyUseConnectionFile değerini göster
                Console.WriteLine("Initial OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Yeni bir OnlyUseConnectionFile değeri ayarla (okuma-yazma olduğu için)
                connection.OnlyUseConnectionFile = true;
                Console.WriteLine("Updated OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Değeri değiştirerek ayar yeteneğini göster
                connection.OnlyUseConnectionFile = !connection.OnlyUseConnectionFile;
                Console.WriteLine("Toggled OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("OnlyUseConnectionFileDemo.xlsx");
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


