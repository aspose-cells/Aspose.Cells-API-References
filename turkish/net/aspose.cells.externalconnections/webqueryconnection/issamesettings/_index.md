---
title: "WebQueryConnection.IsSameSettings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. PRE bloğu içindeki tüm tabloların, ilk satırla aynı genişlik ayarlarıyla ayrıştırılıp ayrıştırılmayacağını belirten bayrak"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/issamesettings/
---
## WebQueryConnection.IsSameSettings property

İlk satırın aynı genişlik ayarlarıyla PRE bloğu içindeki tüm tabloların ayrılıp ayrılmayacağını gösteren işaret.

```csharp
public bool IsSameSettings { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsSameSettingsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Mevcutsa ilk mevcut web sorgu bağlantısına erişin
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // İlk IsSameSettings değerini göster
                    Console.WriteLine("Initial IsSameSettings value: " + connection.IsSameSettings);
                    
                    // IsSameSettings'i true olarak ayarla (çünkü okuma-yazma özelliğine sahip)
                    connection.IsSameSettings = true;
                    Console.WriteLine("Updated IsSameSettings value: " + connection.IsSameSettings);
                    
                    // IsSameSettings'i false olarak geri ayarla
                    connection.IsSameSettings = false;
                    Console.WriteLine("Final IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionIsSameSettingsDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
                }
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


