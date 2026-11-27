---
title: "CustomImplementationFactory.CreateRandomInstance"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomImplementationFactory metod. Skapa en instans av slumpgeneratorn"
type: docs
url: /sv/net/aspose.cells/customimplementationfactory/createrandominstance/
---
## CustomImplementationFactory.CreateRandomInstance method

Skapa en instans av en slumptalsgenerator.

```csharp
public virtual Random CreateRandomInstance()
```

### Returvärde

instans av slumpgeneratorn

### Exempel

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
                // Skapa en instans av CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Anropa CreateRandomInstance för att få ett Random-objekt
                Random random = factory.CreateRandomInstance();

                // Demonstrera funktionaliteten hos Random-instansen
                Console.WriteLine("Random instance created successfully.");
                Console.WriteLine($"Sample random number: {random.Next(1, 100)}");
                Console.WriteLine($"Sample random double: {random.NextDouble():F4}");

                // Visa att fabriken kan användas med CellsHelper
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

### Se även

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


