---
title: "CellsHelper.CustomImplementationFactory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsHelper-egenskap. Hämtar eller anger fabriken för att skapa instanser med speciell implementation"
type: docs
url: /sv/net/aspose.cells/cellshelper/customimplementationfactory/
---
## CellsHelper.CustomImplementationFactory property

Hämtar eller anger fabriken för att skapa instanser med speciell implementation.

```csharp
public static CustomImplementationFactory CustomImplementationFactory { get; set; }
```

### Exempel

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
            // Skapa en instans av CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Demonstrera fabriksmetoder
            MemoryStream memoryStream = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            MemoryStream sizedStream = factory.CreateMemoryStream(1024);
            Console.WriteLine("MemoryStream created with capacity: 1024");

            CultureInfo culture = factory.CreateCultureInfo(1033);
            Console.WriteLine($"CultureInfo created: {culture.DisplayName}");

            Random random = factory.CreateRandomInstance();
            Console.WriteLine($"Random number generated: {random.Next()}");

            // Ställ in fabriken i CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper");
        }
    }
}
```

### Se även

* class [CustomImplementationFactory](../../customimplementationfactory/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


