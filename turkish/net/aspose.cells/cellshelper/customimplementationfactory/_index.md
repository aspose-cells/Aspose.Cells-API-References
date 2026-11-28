---
title: "CellsHelper.CustomImplementationFactory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper özelliği. Özel uygulama ile örnekler oluşturmak için fabrikayı alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/cellshelper/customimplementationfactory/
---
## CellsHelper.CustomImplementationFactory property

Özel uygulama ile örnekler oluşturmak için fabrikayı alır veya ayarlar.

```csharp
public static CustomImplementationFactory CustomImplementationFactory { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperPropertyCustomImplementationFactoryDemo
    {
        public static void Run()
        {
            // CustomImplementationFactory bir örneği oluşturun
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Fabrika yöntemlerini gösterin
            MemoryStream memoryStream = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            MemoryStream sizedStream = factory.CreateMemoryStream(1024);
            Console.WriteLine("MemoryStream created with capacity: 1024");

            CultureInfo culture = factory.CreateCultureInfo(1033);
            Console.WriteLine($"CultureInfo created: {culture.DisplayName}");

            Random random = factory.CreateRandomInstance();
            Console.WriteLine($"Random number generated: {random.Next()}");

            // CellsHelper içinde fabrikayı ayarlayın
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper");
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomImplementationFactory](../../customimplementationfactory/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


