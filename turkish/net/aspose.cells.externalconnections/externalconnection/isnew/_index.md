---
title: "ExternalConnection.IsNew"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bağlantı ilk kez yenilenmemişse doğru, aksi takdirde yanlış. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda oluşabilir."
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/isnew/
---
## ExternalConnection.IsNew property

Bağlantı ilk kez yenilenmemişse true; aksi takdirde false. Bu durum, kullanıcının sorgu tamamlanmadan dosyayı kaydetmesi durumunda ortaya çıkabilir.

```csharp
public bool IsNew { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsNewDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya erişin (yeni oluşturulan bağlantılar genellikle "IsNew" olur)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // İlk IsNew değerini gösterin
                Console.WriteLine("Initial IsNew value: " + connection.IsNew);
                
                // IsNew okunabilir-yazılabilir olduğundan, ayarlamayı gösterin
                connection.IsNew = false;
                Console.WriteLine("Updated IsNew value: " + connection.IsNew);
                
                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("IsNewDemo.xlsx");
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


