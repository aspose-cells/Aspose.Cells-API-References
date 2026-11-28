---
title: "CustomImplementationFactory.CreateRandomInstance"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CustomImplementationFactory yöntemi. Bir rastgele sayı üreteci örneği oluşturur"
type: docs
url: /tr/net/aspose.cells/customimplementationfactory/createrandominstance/
---
## CustomImplementationFactory.CreateRandomInstance method

Rastgele sayı üreteci bir örneği oluşturun.

```csharp
public virtual Random CreateRandomInstance()
```

### Dönüş Değeri

rastgele sayı üreteci örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomImplementationFactoryMethodCreateRandomInstanceDemo
    {
        public static void Run()
        {
            try
            {
                // CustomImplementationFactory bir örneği oluşturun
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Random nesnesi elde etmek için CreateRandomInstance'ı çağırın
                Random random = factory.CreateRandomInstance();

                // Random örneğinin işlevselliğini gösterin
                Console.WriteLine("Random instance created successfully.");
                Console.WriteLine($"Sample random number: {random.Next(1, 100)}");
                Console.WriteLine($"Sample random double: {random.NextDouble():F4}");

                // Fabrikanın CellsHelper ile kullanılabileceğini gösterin
                CellsHelper.CustomImplementationFactory = factory;
                Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateRandomInstance: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


