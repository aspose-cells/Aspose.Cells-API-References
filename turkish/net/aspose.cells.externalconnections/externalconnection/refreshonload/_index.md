---
title: "ExternalConnection.RefreshOnLoad"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bu bağlantının dosya açıldığında yenilenmesi gerekiyorsa doğru, aksi takdirde yanlış."
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/refreshonload/
---
## ExternalConnection.RefreshOnLoad property

Dosya açıldığında bu bağlantının yenilenmesi gerekiyorsa doğru; aksi takdirde yanlış.

```csharp
public bool RefreshOnLoad { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshOnLoadDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya eriş (çalışma kitabı varsayılan bağlantılarla gelir)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // İlk RefreshOnLoad değerini göster
                Console.WriteLine("Initial RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Özelliği ayarlamayı gösterin (okuma-yazma olduğu için)
                connection.RefreshOnLoad = !connection.RefreshOnLoad;
                Console.WriteLine("Updated RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Değiştirilmiş bağlantı ayarlarıyla çalışma kitabını kaydedin
                workbook.Save("RefreshOnLoadDemo.xlsx");
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


