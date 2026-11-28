---
title: "ExternalConnectionCollection.GetExternalConnectionById"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnectionCollection yöntemi. Belirtilen kimliğe sahip ExternalConnection öğesini alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/
---
## ExternalConnectionCollection.GetExternalConnectionById method

Belirtilen kimliğe sahip [`ExternalConnection`](../../externalconnection/) öğesini alır.

```csharp
public ExternalConnection GetExternalConnectionById(int connId)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| connId | Int32 | harici bağlantı kimliği |

### Dönüş Değeri

Belirtilen kimliğe sahip öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionCollectionMethodGetExternalConnectionByIdWithInt32Demo
    {
        public static void Run()
        {
            // Örnek veri bağlantılarıyla yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Harici bağlantı koleksiyonunu al
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Uygun API yöntemlerini kullanarak bağlantılar oluştur ve ekle
            // Not: Gerçek kullanımda, genellikle mevcut bağlantıları alırsınız
            // bu şekilde yeni bağlantılar oluşturmak yerine
            int connectionId1 = 1;
            int connectionId2 = 2;
            
            // Belirli bağlantıyı ID ile al (ilk başta null olacaktır)
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(connectionId1);
            
            if (specificConn == null)
            {
                Console.WriteLine($"No connection found with ID {connectionId1}");
                // Gerçek kullanımda, mevcut bağlantılarla çalışırsınız
                // veya onları uygun API yöntemleriyle oluşturun
            }
            else
            {
                Console.WriteLine($"Found connection: ID={specificConn.ConnectionId}, Name={specificConn.Name}");
                specificConn.Name = "ModifiedConnection";
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


