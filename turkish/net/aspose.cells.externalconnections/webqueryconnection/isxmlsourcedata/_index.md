---
title: "WebQueryConnection.IsXmlSourceData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. XML kaynak verisinin HTML tablosu yerine içe aktarılması gerektiğini gösteren işaret"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/
---
## WebQueryConnection.IsXmlSourceData property

HTML tablosu yerine XML kaynak verisinin içe aktarılması gerektiğini gösteren bayrak.

```csharp
public bool IsXmlSourceData { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXmlSourceDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Mevcut bir web sorgu bağlantısına erişin veya uygun başlatma ile bir tane oluşturun
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // İlk IsXmlSourceData değerini gösterin
                    Console.WriteLine("Initial IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // IsXmlSourceData'yı true olarak ayarlayın
                    connection.IsXmlSourceData = true;
                    Console.WriteLine("Updated IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // IsXmlSourceData'yı false olarak geri ayarlayın
                    connection.IsXmlSourceData = false;
                    Console.WriteLine("Final IsXmlSourceData value: " + connection.IsXmlSourceData);
                    
                    // Çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionIsXmlSourceDataDemo.xlsx");
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


