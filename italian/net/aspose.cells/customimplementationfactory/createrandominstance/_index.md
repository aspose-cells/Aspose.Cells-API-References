---
title: "CustomImplementationFactory.CreateRandomInstance"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomImplementationFactory. Crea un'istanza di generatore di numeri casuali"
type: docs
url: /it/net/aspose.cells/customimplementationfactory/createrandominstance/
---
## CustomImplementationFactory.CreateRandomInstance method

Crea un'istanza di generatore di numeri casuali.

```csharp
public virtual Random CreateRandomInstance()
```

### Valore di ritorno

istanza di generatore di numeri casuali

### Esempi

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
                // Crea un'istanza di CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Chiama CreateRandomInstance per ottenere un oggetto Random
                Random random = factory.CreateRandomInstance();

                // Dimostra la funzionalità dell'istanza Random
                Console.WriteLine("Random instance created successfully.");
                Console.WriteLine($"Sample random number: {random.Next(1, 100)}");
                Console.WriteLine($"Sample random double: {random.NextDouble():F4}");

                // Mostra che la factory può essere usata con CellsHelper
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

### Vedi anche

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


