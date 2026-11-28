---
title: "ExternalConnection.SaveData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bağlantı üzerinden alınan dış verinin bir tabloyu doldurmak için çalışma kitabıyla birlikte kaydedilmesi gerekiyorsa doğru, aksi takdirde yanlış"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/savedata/
---
## ExternalConnection.SaveData property

Bağlantı üzerinden alınan ve bir tabloyu doldurmak için kullanılan harici veriler çalışma kitabı ile birlikte kaydedilecekse doğru; aksi takdirde yanlış.

```csharp
public bool SaveData { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySaveDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya erişin (var olduğunu varsayarak)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Mevcut SaveData değerini göster
                Console.WriteLine("Initial SaveData value: " + connection.SaveData);
                
                // Özelliği ayarlamayı gösterin (okuma-yazma olduğu için)
                connection.SaveData = !connection.SaveData;
                Console.WriteLine("Updated SaveData value: " + connection.SaveData);
                
                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("SaveDataDemo.xlsx");
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


