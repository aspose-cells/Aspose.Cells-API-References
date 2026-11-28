---
title: "WebQueryConnection.ClassType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WebQueryConnection özelliği. Bu ExternalConnection nesnesinin tipini alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/webqueryconnection/classtype/
---
## WebQueryConnection.ClassType property

Bu [`ExternalConnection`](../../externalconnection/) nesnesinin tipini alır.

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyClassTypeDemo
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
                    // ClassType değerini gösterin (yalnızca okuma özelliği)
                    Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
                    
                    // Web sorgusu için beklenen enum değerini doğrula
                    Console.WriteLine("Expected WebQuery enum value: " + 
                        (connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
                    
                    // Çalışma kitabını kaydedin
                    workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


