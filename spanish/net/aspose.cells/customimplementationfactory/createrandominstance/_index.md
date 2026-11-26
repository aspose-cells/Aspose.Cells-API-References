---
title: "CustomImplementationFactory.CreateRandomInstance"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomImplementationFactory. Crea una instancia de generador de números aleatorios"
type: docs
url: /es/net/aspose.cells/customimplementationfactory/createrandominstance/
---
## CustomImplementationFactory.CreateRandomInstance method

Crea una instancia de generador de números aleatorios.

```csharp
public virtual Random CreateRandomInstance()
```

### Valor de retorno

instancia de generador de números aleatorios

### Ejemplos

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
                // Crea una instancia de CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Llama a CreateRandomInstance para obtener un objeto Random
                Random random = factory.CreateRandomInstance();

                // Demuestra la funcionalidad de la instancia Random
                Console.WriteLine("Random instance created successfully.");
                Console.WriteLine($"Sample random number: {random.Next(1, 100)}");
                Console.WriteLine($"Sample random double: {random.NextDouble():F4}");

                // Muestra que la fábrica puede usarse con CellsHelper
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

### Ver también

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


