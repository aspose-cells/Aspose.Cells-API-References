---
title: "Sınıf CustomImplementationFactory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CustomImplementationFactory sınıfı. Kullanıcı tarafından özel bir amaç için yeniden uygulanabilecek bazı örnekleri oluşturmak için fabrika"
type: docs
url: /tr/net/aspose.cells/customimplementationfactory/
---
## CustomImplementationFactory class

Kullanıcı tarafından özel bir amaç için yeniden uygulanabilecek bazı örnekleri oluşturmak için fabrika.

```csharp
public class CustomImplementationFactory
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CustomImplementationFactory](customimplementationfactory/)() | Varsayılan yapıcı. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| virtual [CreateCultureInfo](../../aspose.cells/customimplementationfactory/createcultureinfo/)(int) | Verilen kimliğe göre bir CultureInfo oluşturun. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream)() | MemoryStream'in bir örneğini veya MemoryStream'in özel bir uygulamasını oluşturun. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream_1)(int) | MemoryStream'in bir örneğini veya MemoryStream'in özel bir uygulamasını oluşturun. |
| virtual [CreateRandomInstance](../../aspose.cells/customimplementationfactory/createrandominstance/)() | Rastgele sayı üreteci bir örneği oluşturun. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Globalization;
    using System.IO;

    public class CustomImplementationFactoryDemo
    {
        public static void CustomImplementationFactoryExample()
        {
            // CustomImplementationFactory bir örneği oluşturun
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Parametresiz CreateMemoryStream yöntemini gösterin
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // Kapasite parametresiyle CreateMemoryStream yöntemini gösterin
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // CreateCultureInfo yöntemini gösterin
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // CreateRandomInstance yöntemini gösterin
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // CellsHelper ile fabrikanın örnek kullanımı
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


