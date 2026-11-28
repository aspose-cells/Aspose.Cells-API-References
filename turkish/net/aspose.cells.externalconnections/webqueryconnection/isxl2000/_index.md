---
title: "WebQueryConnection.IsXl2000"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 2000 veya daha yeni bir elektronik tablo uygulamasında yenilendiğinde true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir."
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/isxl2000/
---
## WebQueryConnection.IsXl2000 property

Bu bayrak, daha eski mevcut elektronik tablo dosyalarıyla geriye dönük uyumluluk sağlamak için bulunur ve bu web sorgusu Microsoft Excel 2000 veya daha yeni bir elektronik tablo uygulamasında yenilendiğinde true olarak ayarlanır. Bu, göz ardı edilebilecek isteğe bağlı bir özelliktir.

```csharp
public bool IsXl2000 { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl2000Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Mevcut ilk web sorgu bağlantısına erişin (varsa)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // İlk IsXl2000 değerini göster
                    Console.WriteLine("Initial IsXl2000 value: " + connection.IsXl2000);

                    // IsXl2000'yi true olarak ayarla (çünkü okuma-yazma özelliğine sahip)
                    connection.IsXl2000 = true;
                    Console.WriteLine("Updated IsXl2000 value: " + connection.IsXl2000);

                    // IsXl2000'yi tekrar false olarak ayarla
                    connection.IsXl2000 = false;
                    Console.WriteLine("Final IsXl2000 value: " + connection.IsXl2000);

                    // Çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionIsXl2000Demo.xlsx");
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


