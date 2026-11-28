---
title: "ExternalConnectionCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ExternalConnectionCollection özelliği. Belirtilen indeksteki ExternalConnection öğesini alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

Belirtilen indeksteki [`ExternalConnection`](../../externalconnection/) öğesini alır.

```csharp
public ExternalConnection this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            try
            {
                // Harici bağlantı koleksiyonuna eriş
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Herhangi bir bağlantı olup olmadığını kontrol et
                if (connections.Count > 0)
                {
                    // Bir öğeye indeksle erişimi göster (okuma işlemi)
                    ExternalConnection connection = connections[0];

                    // Bağlantı bilgilerini görüntüleyin
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                    Console.WriteLine($"Connection ID: {connection.ConnectionId}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("ExternalConnectionItemDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

Belirtilen adla [`ExternalConnection`](../../externalconnection/) öğesini alır.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| connectionName | veri bağlantısının adı |

### Dönüş Değeri

Belirtilen ada sahip öğe.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // Harici bağlantı koleksiyonuna eriş
                ExternalConnectionCollection connections = workbook.DataConnections;
                
                // Örnek bir bağlantı ekle (gösterim için gerekliyse)
                // Bu, koleksiyonun bağlantı eklemeye izin verdiğini varsayar
                // connections.Add(new ExternalConnection());
                
                // Bir öğeye adla erişimi göster (okuma işlemi)
                // Not: Gerçek bir senaryoda, gerçek bağlantı adlarına ihtiyacınız olur
                if (connections.Count > 0)
                {
                    // İlk bağlantı adını al (varsa)
                    string connectionName = connections[0].Name;
                    
                    // Item özelliğine eriş
                    ExternalConnection connection = connections[connectionName];
                    
                    // Bağlantı bilgilerini görüntüleyin
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


