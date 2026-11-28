---
title: "ConnectionParameterCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConnectionParameterCollection özelliği. Belirtilen indeksteki ConnectionParameter öğesini alır"
type: docs
url: /tr/net/aspose.cells.externalconnections/connectionparametercollection/item/
---
## ConnectionParameterCollection indexer (1 of 2)

Belirtilen indeksteki [`ConnectionParameter`](../../connectionparameter/) öğesini alır.

```csharp
public ConnectionParameter this[int index] { get; }
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

    public class ConnectionParameterCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk harici bağlantıyı al
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Parametreler koleksiyonunu al
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Erişmeden önce herhangi bir parametre olup olmadığını kontrol et
                if (parameters.Count > 0)
                {
                    // Item özelliğini okuma örneği göster
                    ConnectionParameter firstParam = parameters[0];
                    Console.WriteLine($"Parameter type: {firstParam.GetType().Name}");
                }
                else
                {
                    Console.WriteLine("No parameters in collection");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterItemDemo.xlsx");
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

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ConnectionParameterCollection indexer (2 of 2)

Belirtilen adla [`ConnectionParameter`](../../connectionparameter/) öğesini alır.

```csharp
public ConnectionParameter this[string connParamName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| connParamName | bağlantı parametresi adı |

### Dönüş Değeri

Belirtilen ada sahip öğe.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            try
            {
                // İlk harici bağlantıyı al
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Parametreler koleksiyonunu al
                ConnectionParameterCollection parameters = connection.Parameters;
                
                // Item özelliğini göstermek için mevcut parametrelerin olup olmadığını kontrol et
                if (parameters.Count == 0)
                {
                    Console.WriteLine("No parameters in collection to demonstrate Item property");
                    return;
                }
                
                // Demonstrasyon için kullanılacak ilk parametrenin adını al
                string firstParamName = parameters[0].Name;
                
                // Item özelliğini ad ile okuma örneği göster
                ConnectionParameter retrievedParam = parameters[firstParamName];
                
                if (retrievedParam != null)
                {
                    Console.WriteLine($"Retrieved parameter name: {retrievedParam.Name}");
                }
                else
                {
                    Console.WriteLine("Parameter not found");
                }
                
                // Çalışma kitabını kaydedin
                workbook.Save("ConnectionParameterItemDemo.xlsx");
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

* class [ConnectionParameter](../../connectionparameter/)
* class [ConnectionParameterCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


