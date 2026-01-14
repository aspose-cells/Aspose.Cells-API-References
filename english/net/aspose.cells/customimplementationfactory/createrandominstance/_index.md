---
title: CustomImplementationFactory.CreateRandomInstance
second_title: Aspose.Cells for .NET API Reference
description: CustomImplementationFactory method. Create one instance of random number generator
type: docs
url: /net/aspose.cells/customimplementationfactory/createrandominstance/
---
## CustomImplementationFactory.CreateRandomInstance method

Create one instance of random number generator.

```csharp
public virtual Random CreateRandomInstance()
```

### Return Value

instance of random number generator

### Examples

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
                // Create an instance of CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Call CreateRandomInstance to get a Random object
                Random random = factory.CreateRandomInstance();

                // Demonstrate the functionality of the Random instance
                Console.WriteLine("Random instance created successfully.");
                Console.WriteLine($"Sample random number: {random.Next(1, 100)}");
                Console.WriteLine($"Sample random double: {random.NextDouble():F4}");

                // Show that the factory can be used with CellsHelper
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

### See Also

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


