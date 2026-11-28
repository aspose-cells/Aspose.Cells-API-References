---
title: "WebQueryConnection.IsXl97"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 97'de oluşturulduysa true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir."
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/isxl97/
---
## WebQueryConnection.IsXl97 property

Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 97'de oluşturulduğunda true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir.

```csharp
public bool IsXl97 { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl97Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Örneği anlamlı kılmak için bazı verilerle bir çalışma sayfası oluşturun
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Data";
                
                // Mevcut bir dosyadan yükleyerek veya uygun şekilde oluşturarak bir web sorgu bağlantısı oluşturun
                // WebQueryConnection'ı doğrudan oluşturamadığımız için mevcut bir tanesine erişeceğiz
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // İlk IsXl97 değerini göster
                    Console.WriteLine("Initial IsXl97 value: " + connection.IsXl97);
                    
                    // IsXl97'yi true olarak ayarla (çünkü okuma-yazma özelliğine sahip)
                    connection.IsXl97 = true;
                    Console.WriteLine("Updated IsXl97 value: " + connection.IsXl97);
                    
                    // IsXl97'yi tekrar false olarak ayarla
                    connection.IsXl97 = false;
                    Console.WriteLine("Final IsXl97 value: " + connection.IsXl97);
                    
                    // Çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionIsXl97Demo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
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


