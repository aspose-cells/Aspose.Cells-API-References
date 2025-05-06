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
// Called: Random random = factory.CreateRandomInstance();
public static void Method_CreateRandomInstance()
        {
            // Create an instance of CustomImplementationFactory
            CustomImplementationFactory factory = new CustomImplementationFactory();

            // Demonstrate the CreateMemoryStream method without parameters
            MemoryStream memoryStream1 = factory.CreateMemoryStream();
            Console.WriteLine(&quot;MemoryStream created without parameters.&quot;);

            // Demonstrate the CreateMemoryStream method with capacity parameter
            int capacity = 1024;
            MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
            Console.WriteLine($&quot;MemoryStream created with capacity: {capacity}.&quot;);

            // Demonstrate the CreateCultureInfo method
            int lcid = 1033; // LCID for English - United States
            CultureInfo cultureInfo = factory.CreateCultureInfo(lcid);
            Console.WriteLine($&quot;CultureInfo created with LCID: {lcid}.&quot;);

            // Demonstrate the CreateRandomInstance method
            Random random = factory.CreateRandomInstance();
            Console.WriteLine(&quot;Random instance created.&quot;);

            // Example usage of the factory with CellsHelper
            CellsHelper.CustomImplementationFactory = factory;
            Console.WriteLine(&quot;CustomImplementationFactory set in CellsHelper.&quot;);
        }
```

### See Also

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


