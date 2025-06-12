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
using System;
using System.IO;
using System.Globalization;

namespace AsposeCellsExamples
{
    public class CustomImplementationFactory2
    {
        public MemoryStream CreateMemoryStream()
        {
            return new MemoryStream();
        }

        public MemoryStream CreateMemoryStream(int capacity)
        {
            return new MemoryStream(capacity);
        }

        public CultureInfo CreateCultureInfo(int lcid)
        {
            return new CultureInfo(lcid);
        }

        public Random CreateRandomInstance()
        {
            return new Random();
        }
    }

    public class CustomImplementationFactory2MethodCreateMemoryStreamDemo
    {
        public static void Run()
        {
            CustomImplementationFactory2 factory = new CustomImplementationFactory2();

            // Create MemoryStream without parameters
            using (MemoryStream stream1 = factory.CreateMemoryStream())
            {
                Console.WriteLine($"MemoryStream created - Length: {stream1.Length}, Capacity: {stream1.Capacity}");
            }

            // Create MemoryStream with capacity
            using (MemoryStream stream2 = factory.CreateMemoryStream(1024))
            {
                Console.WriteLine($"MemoryStream created - Length: {stream2.Length}, Capacity: {stream2.Capacity}");
            }
        }
    }
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
using System;
using System.IO;
using System.Globalization;

namespace AsposeCellsExamples
{
    public interface ICustomImplementationFactory
    {
        MemoryStream CreateMemoryStream();
        MemoryStream CreateMemoryStream(int capacity);
        CultureInfo CreateCultureInfo(int lcid);
        Random CreateRandomInstance();
    }

    public class CustomImplementationFactory : ICustomImplementationFactory
    {
        public MemoryStream CreateMemoryStream()
        {
            return new MemoryStream();
        }

        public MemoryStream CreateMemoryStream(int capacity)
        {
            return new MemoryStream(capacity);
        }

        public CultureInfo CreateCultureInfo(int lcid)
        {
            return new CultureInfo(lcid);
        }

        public Random CreateRandomInstance()
        {
            return new Random();
        }
    }

    public class CustomImplementationFactoryMethodCreateMemoryStreamWithInt32Demo
    {
        public static void Run()
        {
            CustomImplementationFactory factory = new CustomImplementationFactory();
            
            // Demonstrate CreateMemoryStream with capacity parameter
            int capacity = 1024;
            using (MemoryStream memoryStream = factory.CreateMemoryStream(capacity))
            {
                Console.WriteLine($"MemoryStream created with capacity: {capacity}, Length: {memoryStream.Length}");
            }
        }
    }
}
```

### See Also

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


