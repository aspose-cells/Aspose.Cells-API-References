---
title: "CellsHelper.CustomImplementationFactory"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CellsHelper-Eigenschaft. Liest oder legt die Fabrik fest, die Instanzen mit spezieller Implementierung erstellt"
type: docs
url: /de/net/aspose.cells/cellshelper/customimplementationfactory/
---
## CellsHelper.CustomImplementationFactory property

Liest oder setzt die Fabrik zum Erzeugen von Instanzen mit spezieller Implementierung.

```csharp
public static CustomImplementationFactory CustomImplementationFactory { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine Instanz von CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Demonstrieren Sie Fabrikmethoden
            MemoryStream memoryStream = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            MemoryStream sizedStream = factory.CreateMemoryStream(1024);
            Console.WriteLine("MemoryStream created with capacity: 1024");

            CultureInfo culture = factory.CreateCultureInfo(1033);
            Console.WriteLine($"CultureInfo created: {culture.DisplayName}");

            Random random = factory.CreateRandomInstance();
            Console.WriteLine($"Random number generated: {random.Next()}");

            // Setzen Sie die Fabrik in CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper");
        }
    }
}
```

### Siehe auch

* class [CustomImplementationFactory](../../customimplementationfactory/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


