---
title: "ExternalConnection.ConnectionId"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnection özelliği. Bu bağlantının benzersiz tanımlayıcısını belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnection/connectionid/
---
## ExternalConnection.ConnectionId property

Bu bağlantının benzersiz tanımlayıcısını belirtir.

```csharp
[Obsolete("Use ExternalConnection.Id property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ConnectionId { get; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExternalConnection.Id özelliğini kullanın. Bu özellik, Ekim 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // İlk dış bağlantıya eriş (çalışma kitabı varsayılan bağlantılarla gelir)
                ExternalConnection connection = workbook.DataConnections[0];

                // ConnectionId değerini göster (yalnızca okuma özelliği)
                Console.WriteLine("ConnectionId value: " + connection.ConnectionId);

                // Karşılaştırma için Id değerini göster (aynı zamanda yalnızca okuma)
                Console.WriteLine("Id value: " + connection.Id);

                // Her iki özelliğin de yalnızca okunabilir olduğunu, onları göstermeye çalışarak gösterin
                Console.WriteLine("ConnectionId and Id are both read-only properties");
                Console.WriteLine("ConnectionId: " + connection.ConnectionId + ", Id: " + connection.Id);

                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionIdDemo.xlsx");
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


