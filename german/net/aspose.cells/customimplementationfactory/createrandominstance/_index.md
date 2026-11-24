---
title: "CustomImplementationFactory.CreateRandomInstance"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Methode CustomImplementationFactory. Erstellen Sie eine Instanz eines Zufallszahlengenerators"
type: docs
url: /de/net/aspose.cells/customimplementationfactory/createrandominstance/
---
## CustomImplementationFactory.CreateRandomInstance method

Erstellen Sie eine Instanz eines Zufallszahlengenerators.

```csharp
public virtual Random CreateRandomInstance()
```

### Rückgabewert

Instanz eines Zufallszahlengenerators

### Beispiele

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
                // Erstellen Sie eine Instanz von CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Rufen Sie CreateRandomInstance auf, um ein Random-Objekt zu erhalten
                Random random = factory.CreateRandomInstance();

                // Demonstrieren Sie die Funktionalität der Random-Instanz
                Console.WriteLine("Random instance created successfully.");
                Console.WriteLine($"Sample random number: {random.Next(1, 100)}");
                Console.WriteLine($"Sample random double: {random.NextDouble():F4}");

                // Zeigen Sie, dass die Fabrik mit CellsHelper verwendet werden kann
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

### Siehe auch

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


