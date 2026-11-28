---
title: "ExternalConnection.Parameters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. ODBC veya web sorgusu için ConnectionParameterCollection alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/parameters/
---
## ExternalConnection.Parameters property

ODBC veya web sorgusu için [`ConnectionParameterCollection`](../../connectionparametercollection/) alır.

```csharp
public ConnectionParameterCollection Parameters { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyParametersDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk dış bağlantıya erişin (var olduğunu varsayarak)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Parameters koleksiyon bilgilerini görüntüle
                ConnectionParameterCollection parameters = connection.Parameters;
                Console.WriteLine($"Number of parameters: {parameters.Count}");
                
                // Mevcut ise her parametrenin bilgisini görüntüle
                foreach (ConnectionParameter param in parameters)
                {
                    Console.WriteLine($"Parameter name: {param.Name}");
                    Console.WriteLine($"Parameter type: {param.Type}");
                    Console.WriteLine($"Parameter prompt: {param.Prompt}");
                    Console.WriteLine("----------------------");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ParametersDemo.xlsx");
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

* class [ConnectionParameterCollection](../../connectionparametercollection/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


