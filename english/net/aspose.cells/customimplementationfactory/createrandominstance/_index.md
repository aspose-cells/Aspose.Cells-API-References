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
using System;
using System.IO;
using System.Globalization;

namespace AsposeCellsExamples
{
    public class CustomImplementationFactory1
    {
        public MemoryStream CreateMemoryStream()
        => new MemoryStream();

        public MemoryStream CreateMemoryStream(int capacity)
            => new MemoryStream(capacity);

        public CultureInfo CreateCultureInfo(int lcid)
            => new CultureInfo(lcid);

        public Random CreateRandomInstance()
            => new Random();
    }

    public static class CellsHelper
    {
        public static CustomImplementationFactory1 CustomImplementationFactory { get; set; }
    }

    public class CustomImplementationFactory1MethodCreateRandomInstanceDemo
    {
        public static void Run()
        {
            CustomImplementationFactory1 factory = new CustomImplementationFactory1();

            // Create and demonstrate Random instance
            Random random = factory.CreateRandomInstance();
            Console.WriteLine($"Random number: {random.Next()}");

            // Set factory in CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("Factory set in CellsHelper");
        }
    }
}
```

### See Also

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


