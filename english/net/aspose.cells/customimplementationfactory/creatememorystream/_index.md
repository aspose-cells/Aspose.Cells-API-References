---
title: CustomImplementationFactory.CreateMemoryStream
second_title: Aspose.Cells for .NET API Reference
description: CustomImplementationFactory method. Create one instance of MemoryStream or custom implementation of MemoryStream
type: docs
url: /net/aspose.cells/customimplementationfactory/creatememorystream/
---
## CreateMemoryStream() {#creatememorystream}

Create one instance of MemoryStream or custom implementation of MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream()
```

### Return Value

The MemoryStream instance.

### Examples

```csharp
// Called: var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
public static void Method_CreateMemoryStream()
        {
            // Setting properties of CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = &quot;C:\\Program Files\\Aspose\\Cells&quot;;
            CellsHelper.AltStartPath = &quot;D:\\Aspose\\Cells&quot;;
            CellsHelper.LibraryPath = &quot;E:\\Aspose\\Cells\\Library&quot;;
            CellsHelper.IsCloudPlatform = true;

            // Assuming CustomImplementationFactory is already defined and instantiated elsewhere
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // Demonstrating the use of CellsHelper properties
            Console.WriteLine(&quot;Significant Digits: &quot; + CellsHelper.SignificantDigits);
            Console.WriteLine(&quot;DPI: &quot; + CellsHelper.DPI);
            Console.WriteLine(&quot;Startup Path: &quot; + CellsHelper.StartupPath);
            Console.WriteLine(&quot;Alternate Startup Path: &quot; + CellsHelper.AltStartPath);
            Console.WriteLine(&quot;Library Path: &quot; + CellsHelper.LibraryPath);
            Console.WriteLine(&quot;Is Cloud Platform: &quot; + CellsHelper.IsCloudPlatform);

            // Example of using CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine(&quot;MemoryStream created with CustomImplementationFactory: &quot; + (memoryStream != null));

            return;
        }
```

### See Also

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateMemoryStream(int) {#creatememorystream_1}

Create one instance of MemoryStream or custom implementation of MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream(int capacity)
```

| Parameter | Type | Description |
| --- | --- | --- |
| capacity | Int32 | Initial capacity for the MemoryStream |

### Return Value

The MemoryStream instance.

### Examples

```csharp
// Called: MemoryStream memoryStream2 = factory.CreateMemoryStream(capacity);
public static void Method_Int32_()
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


