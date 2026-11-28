---
title: "ExternalConnection.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bağlantının kimliğini alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

Bağlantının kimliğini alır.

```csharp
public int Id { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // İlk dış bağlantıya eriş (çalışma kitabı varsayılan bağlantılarla gelir)
                ExternalConnection connection = workbook.DataConnections[0];

                // Mevcut Id değerini göster (yalnızca okuma özelliği)
                Console.WriteLine("External Connection Id: " + connection.Id);

                // Bağlam için diğer yalnızca okunabilir özellikleri göster
                Console.WriteLine("Connection Class Type: " + connection.ClassType);
                Console.WriteLine("Connection Name: " + connection.Name);

                // Çalışma kitabını kaydedin
                workbook.Save("ExternalConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with connection Id: " + connection.Id);
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


