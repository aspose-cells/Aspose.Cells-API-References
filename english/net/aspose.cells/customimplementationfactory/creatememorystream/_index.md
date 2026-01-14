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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomImplementationFactoryMethodCreateMemoryStreamDemo
    {
        public static void Run()
        {
            try
            {
                // Create an instance of CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Demonstrate CreateMemoryStream without parameters
                MemoryStream stream1 = factory.CreateMemoryStream();
                Console.WriteLine($"MemoryStream created with default capacity. Length: {stream1.Length}");

                // Demonstrate CreateMemoryStream with capacity parameter
                int capacity = 2048;
                MemoryStream stream2 = factory.CreateMemoryStream(capacity);
                Console.WriteLine($"MemoryStream created with capacity: {capacity}. Length: {stream2.Length}");

                // Write some data to demonstrate functionality
                byte[] data = System.Text.Encoding.UTF8.GetBytes("Sample data for MemoryStream");
                stream2.Write(data, 0, data.Length);
                Console.WriteLine($"Data written to MemoryStream. New length: {stream2.Length}");

                // Reset position for potential reading
                stream2.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CreateMemoryStream demonstration: {ex.Message}");
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CustomImplementationFactoryMethodCreateMemoryStreamWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Create an instance of CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Call CreateMemoryStream with a capacity parameter
                int capacity = 4096;
                MemoryStream memoryStream = factory.CreateMemoryStream(capacity);

                // Display information about the created MemoryStream
                Console.WriteLine($"MemoryStream created successfully with capacity: {capacity}");
                Console.WriteLine($"Initial length: {memoryStream.Length}");
                Console.WriteLine($"Initial capacity: {memoryStream.Capacity}");

                // Write some sample data to demonstrate functionality
                byte[] sampleData = System.Text.Encoding.UTF8.GetBytes("Test data for MemoryStream");
                memoryStream.Write(sampleData, 0, sampleData.Length);
                Console.WriteLine($"Data written. New length: {memoryStream.Length}");

                // Reset position for potential reading
                memoryStream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling CreateMemoryStream: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


