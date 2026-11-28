---
title: "Enum ReConnectionMethodType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.ReConnectionMethodType enum. Bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir"
type: docs
url: /tr/net/aspose.cells.externalconnections/reconnectionmethodtype/
---
## ReConnectionMethodType enumeration

Bağlantı başarısız olduğunda elektronik tablo uygulamasının ne yapması gerektiğini belirtir.

```csharp
public enum ReConnectionMethodType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Required | `1` | Yenileme sırasında mevcut bağlantı bilgilerini kullan ve eğer geçersiz hale gelirse, harici bağlantı dosyasından mevcutsa güncellenmiş bağlantı bilgilerini al. |
| Always | `2` | Her yenilemede, mevcutsa harici bağlantı dosyasından güncellenmiş bağlantı bilgilerini al ve bunları mevcut bağlantı bilgileri yerine kullan. Bu durumda harici bağlantı dosyası mevcut değilse veri yenilemesi başarısız olur. |
| Never | `3` | Harici bağlantı dosyasından, mevcut olsa ve mevcut bağlantı bilgileri geçersiz olsa bile, asla güncellenmiş bağlantı bilgisi alınmaz |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassReConnectionMethodTypeDemo
    {
        public static void Run()
        {
            try
            {
                // ReConnectionMethodType enum değerlerini oluşturma ve kullanma örneği
                ReConnectionMethodType method1 = ReConnectionMethodType.Required;
                ReConnectionMethodType method2 = ReConnectionMethodType.Always;
                ReConnectionMethodType method3 = ReConnectionMethodType.Never;

                Console.WriteLine("ReConnectionMethodType values:");
                Console.WriteLine($"Required: {(int)method1}");
                Console.WriteLine($"Always: {(int)method2}");
                Console.WriteLine($"Never: {(int)method3}");

                // Bir switch ifadesinde kullanımını göster
                Console.WriteLine("\nDemonstrating switch usage:");
                TestConnectionMethod(method1);
                TestConnectionMethod(method2);
                TestConnectionMethod(method3);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReConnectionMethodType: {ex.Message}");
            }
        }

        private static void TestConnectionMethod(ReConnectionMethodType method)
        {
            switch (method)
            {
                case ReConnectionMethodType.Required:
                    Console.WriteLine("Using Required reconnection method");
                    break;
                case ReConnectionMethodType.Always:
                    Console.WriteLine("Using Always reconnection method");
                    break;
                case ReConnectionMethodType.Never:
                    Console.WriteLine("Using Never reconnection method");
                    break;
                default:
                    Console.WriteLine("Unknown reconnection method");
                    break;
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


