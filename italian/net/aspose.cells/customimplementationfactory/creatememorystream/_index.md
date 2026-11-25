---
title: "CustomImplementationFactory.CreateMemoryStream"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo CustomImplementationFactory. Crea un'istanza di MemoryStream o un'implementazione personalizzata di MemoryStream"
type: docs
url: /it/net/aspose.cells/customimplementationfactory/creatememorystream/
---
## CreateMemoryStream() {#creatememorystream}

Crea un'istanza di MemoryStream o di un'implementazione personalizzata di MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream()
```

### Valore di ritorno

L'istanza di MemoryStream.

### Esempi

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
                // Crea un'istanza di CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Dimostra CreateMemoryStream senza parametri
                MemoryStream stream1 = factory.CreateMemoryStream();
                Console.WriteLine($"MemoryStream created with default capacity. Length: {stream1.Length}");

                // Dimostra CreateMemoryStream con parametro di capacità
                int capacity = 2048;
                MemoryStream stream2 = factory.CreateMemoryStream(capacity);
                Console.WriteLine($"MemoryStream created with capacity: {capacity}. Length: {stream2.Length}");

                // Scrivi alcuni dati per dimostrare la funzionalità
                byte[] data = System.Text.Encoding.UTF8.GetBytes("Sample data for MemoryStream");
                stream2.Write(data, 0, data.Length);
                Console.WriteLine($"Data written to MemoryStream. New length: {stream2.Length}");

                // Reimposta la posizione per una potenziale lettura
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

### Vedi anche

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateMemoryStream(int) {#creatememorystream_1}

Crea un'istanza di MemoryStream o di un'implementazione personalizzata di MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream(int capacity)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| capacità | Int32 | Capacità iniziale per il MemoryStream |

### Valore di ritorno

L'istanza di MemoryStream.

### Esempi

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
                // Crea un'istanza di CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Chiama CreateMemoryStream con un parametro di capacità
                int capacity = 4096;
                MemoryStream memoryStream = factory.CreateMemoryStream(capacity);

                // Visualizza le informazioni sul MemoryStream creato
                Console.WriteLine($"MemoryStream created successfully with capacity: {capacity}");
                Console.WriteLine($"Initial length: {memoryStream.Length}");
                Console.WriteLine($"Initial capacity: {memoryStream.Capacity}");

                // Scrivi alcuni dati di esempio per dimostrare la funzionalità
                byte[] sampleData = System.Text.Encoding.UTF8.GetBytes("Test data for MemoryStream");
                memoryStream.Write(sampleData, 0, sampleData.Length);
                Console.WriteLine($"Data written. New length: {memoryStream.Length}");

                // Reimposta la posizione per una potenziale lettura
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

### Vedi anche

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


