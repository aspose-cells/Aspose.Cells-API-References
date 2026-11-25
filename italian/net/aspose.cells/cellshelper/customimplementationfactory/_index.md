---
title: "CellsHelper.CustomImplementationFactory"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CellsHelper. Ottiene o imposta la factory per creare istanze con implementazione speciale"
type: docs
url: /it/net/aspose.cells/cellshelper/customimplementationfactory/
---
## CellsHelper.CustomImplementationFactory property

Ottiene o imposta la factory per creare istanze con implementazione speciale.

```csharp
public static CustomImplementationFactory CustomImplementationFactory { get; set; }
```

### Esempi

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
            // Crea un'istanza di CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Dimostra i metodi factory
            MemoryStream memoryStream = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            MemoryStream sizedStream = factory.CreateMemoryStream(1024);
            Console.WriteLine("MemoryStream created with capacity: 1024");

            CultureInfo culture = factory.CreateCultureInfo(1033);
            Console.WriteLine($"CultureInfo created: {culture.DisplayName}");

            Random random = factory.CreateRandomInstance();
            Console.WriteLine($"Random number generated: {random.Next()}");

            // Imposta la factory in CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper");
        }
    }
}
```

### Vedi anche

* class [CustomImplementationFactory](../../customimplementationfactory/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


