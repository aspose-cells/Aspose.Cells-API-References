---
title: Class CustomImplementationFactory
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CustomImplementationFactory class. Factory to create some instances which may be reimplemented by the user for a special purpose
type: docs
url: /net/aspose.cells/customimplementationfactory/
---
## CustomImplementationFactory class

Factory to create some instances which may be re-implemented by the user for a special purpose.

```csharp
public class CustomImplementationFactory
```

## Constructors

| Name | Description |
| --- | --- |
| [CustomImplementationFactory](customimplementationfactory/)() | The default constructor. |

## Methods

| Name | Description |
| --- | --- |
| virtual [CreateCultureInfo](../../aspose.cells/customimplementationfactory/createcultureinfo/)(int) | Create one CultureInfo by given id. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream)() | Create one instance of MemoryStream or custom implementation of MemoryStream. |
| virtual [CreateMemoryStream](../../aspose.cells/customimplementationfactory/creatememorystream/#creatememorystream_1)(int) | Create one instance of MemoryStream or custom implementation of MemoryStream. |
| virtual [CreateRandomInstance](../../aspose.cells/customimplementationfactory/createrandominstance/)() | Create one instance of random number generator. |

### Examples

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
            // Create an instance of CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Demonstrate the CreateMemoryStream method without parameters
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created without parameters.");

            // Demonstrate the CreateMemoryStream method with capacity parameter
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($"MemoryStream created with capacity: {capacity}.");

            // Demonstrate the CreateCultureInfo method
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($"CultureInfo created with LCID: {lcid}.");

            // Demonstrate the CreateRandomInstance method
            Random random = factory.CreateRandomInstance();
            Console.WriteLine("Random instance created.");

            // Example usage of the factory with CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine("CustomImplementationFactory set in CellsHelper.");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


