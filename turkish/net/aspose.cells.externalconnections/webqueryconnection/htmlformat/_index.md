---
title: "WebQueryConnection.HtmlFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Web sorgu verilerini çalışma sayfasına getirirken HTML kaynağından gelen biçimlendirmeyi nasıl ele alacağınız. sourceData True olduğunda geçerlidir"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/htmlformat/
---
## WebQueryConnection.HtmlFormat property

HTML kaynağından gelen biçimlendirmeyi, web sorgu verileri çalışma sayfasına getirildiğinde nasıl ele alacağınız. sourceData True olduğunda geçerlidir.

```csharp
public HtmlFormatHandlingType HtmlFormat { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyHtmlFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Mevcut ilk web sorgu bağlantısına erişin (varsa)
            // Veya web bağlantılarını içeren bir dosya yükleyerek yeni bir tane oluşturun
            if (workbook.DataConnections.Count > 0)
            {
                try
                {
                    WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                    
                    // İlk HtmlFormat değerini gösterin
                    Console.WriteLine("Initial HtmlFormat value: " + connection.HtmlFormat);
                    
                    // HtmlFormat'ı Rtf olarak ayarlayın (yazma işlemini gösterir)
                    connection.HtmlFormat = HtmlFormatHandlingType.Rtf;
                    Console.WriteLine("Updated HtmlFormat value: " + connection.HtmlFormat);
                    
                    // HtmlFormat'ı None olarak ayarlayın
                    connection.HtmlFormat = HtmlFormatHandlingType.None;
                    Console.WriteLine("Final HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Web sorgu bağlantısı ile çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionHtmlFormatDemo.xlsx");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error: {ex.Message}");
                }
            }
            else
            {
                Console.WriteLine("No web query connections found in the workbook.");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [HtmlFormatHandlingType](../../htmlformathandlingtype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


