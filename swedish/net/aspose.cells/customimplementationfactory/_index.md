---
title: "Klass CustomImplementationFactory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CustomImplementationFactory klass. Fabrik för att skapa vissa instanser som kan omimplementeras av användaren för ett speciellt ändamål"
type: docs
url: /sv/net/aspose.cells/customimplementationfactory/
---
## CustomImplementationFactory class

Fabrik för att skapa vissa instanser som kan återimplementeras av användaren för ett speciellt ändamål.

```csharp
public class CustomImplementationFactory
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CustomImplementationFactory](customimplementationfactory/)() | Standardkonstruktorn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [CreateCultureInfo](../../aspose.cells/customimplementationfactory/createcultureinfo/)(int) | Skapa en CultureInfo med givet id. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream)() | Skapa en instans av MemoryStream eller en anpassad implementation av MemoryStream. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream_1)(int) | Skapa en instans av MemoryStream eller en anpassad implementation av MemoryStream. |
| virtual [CreateRandomInstance](../../aspose.cells/customimplementationfactory/createrandominstance/)() | Skapa en instans av en slumptalsgenerator. |

### Exempel

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
            // Skapa en instans av CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Demonstrera metoden CreateMemoryStream utan parametrar
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // Demonstrera metoden CreateMemoryStream med kapacitetsparameter
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // Demonstrera metoden CreateCultureInfo
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // Demonstrera metoden CreateRandomInstance
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // Exempel på användning av fabriken med CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


