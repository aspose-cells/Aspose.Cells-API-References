---
title: "CustomImplementationFactory.CreateMemoryStream"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CustomImplementationFactory‑metod. Skapa en instans av MemoryStream eller en anpassad implementation av MemoryStream"
type: docs
url: /sv/net/aspose.cells/customimplementationfactory/creatememorystream/
---
## CreateMemoryStream() {#creatememorystream}

Skapa en instans av MemoryStream eller en anpassad implementation av MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream()
```

### Returvärde

MemoryStream‑instansen.

### Exempel

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
                // Skapa en instans av CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Demonstrera CreateMemoryStream utan parametrar
                MemoryStream stream1 = factory.CreateMemoryStream();
                Console.WriteLine($"MemoryStream created with default capacity. Length: {stream1.Length}");

                // Demonstrera CreateMemoryStream med kapacitetsparameter
                int capacity = 2048;
                MemoryStream stream2 = factory.CreateMemoryStream(capacity);
                Console.WriteLine($"MemoryStream created with capacity: {capacity}. Length: {stream2.Length}");

                // Skriv lite data för att demonstrera funktionaliteten
                byte[] data = System.Text.Encoding.UTF8.GetBytes("Sample data for MemoryStream");
                stream2.Write(data, 0, data.Length);
                Console.WriteLine($"Data written to MemoryStream. New length: {stream2.Length}");

                // Återställ positionen för eventuell läsning
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

### Se även

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateMemoryStream(int) {#creatememorystream_1}

Skapa en instans av MemoryStream eller en anpassad implementation av MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream(int capacity)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kapacitet | Int32 | Initial kapacitet för MemoryStream |

### Returvärde

MemoryStream‑instansen.

### Exempel

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
                // Skapa en instans av CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Anropa CreateMemoryStream med en kapacitetsparameter
                int capacity = 4096;
                MemoryStream memoryStream = factory.CreateMemoryStream(capacity);

                // Visa information om den skapade MemoryStream
                Console.WriteLine($"MemoryStream created successfully with capacity: {capacity}");
                Console.WriteLine($"Initial length: {memoryStream.Length}");
                Console.WriteLine($"Initial capacity: {memoryStream.Capacity}");

                // Skriv exempeldata för att demonstrera funktionaliteten
                byte[] sampleData = System.Text.Encoding.UTF8.GetBytes("Test data for MemoryStream");
                memoryStream.Write(sampleData, 0, sampleData.Length);
                Console.WriteLine($"Data written. New length: {memoryStream.Length}");

                // Återställ positionen för eventuell läsning
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

### Se även

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


