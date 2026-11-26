---
title: "CustomImplementationFactory.CreateMemoryStream"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomImplementationFactory. Crea una instancia de MemoryStream o una implementación personalizada de MemoryStream"
type: docs
url: /es/net/aspose.cells/customimplementationfactory/creatememorystream/
---
## CreateMemoryStream() {#creatememorystream}

Crea una instancia de MemoryStream o de una implementación personalizada de MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream()
```

### Valor de retorno

La instancia MemoryStream.

### Ejemplos

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
                // Crea una instancia de CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Demuestra CreateMemoryStream sin parámetros
                MemoryStream stream1 = factory.CreateMemoryStream();
                Console.WriteLine($"MemoryStream created with default capacity. Length: {stream1.Length}");

                // Demuestra CreateMemoryStream con parámetro de capacidad
                int capacity = 2048;
                MemoryStream stream2 = factory.CreateMemoryStream(capacity);
                Console.WriteLine($"MemoryStream created with capacity: {capacity}. Length: {stream2.Length}");

                // Escribe algunos datos para demostrar la funcionalidad
                byte[] data = System.Text.Encoding.UTF8.GetBytes("Sample data for MemoryStream");
                stream2.Write(data, 0, data.Length);
                Console.WriteLine($"Data written to MemoryStream. New length: {stream2.Length}");

                // Restablece la posición para una posible lectura
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

### Ver también

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateMemoryStream(int) {#creatememorystream_1}

Crea una instancia de MemoryStream o de una implementación personalizada de MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream(int capacity)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| capacidad | Int32 | Capacidad inicial para el MemoryStream |

### Valor de retorno

La instancia MemoryStream.

### Ejemplos

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
                // Crea una instancia de CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Llama a CreateMemoryStream con un parámetro de capacidad
                int capacity = 4096;
                MemoryStream memoryStream = factory.CreateMemoryStream(capacity);

                // Muestra información sobre el MemoryStream creado
                Console.WriteLine($"MemoryStream created successfully with capacity: {capacity}");
                Console.WriteLine($"Initial length: {memoryStream.Length}");
                Console.WriteLine($"Initial capacity: {memoryStream.Capacity}");

                // Escribe algunos datos de muestra para demostrar la funcionalidad
                byte[] sampleData = System.Text.Encoding.UTF8.GetBytes("Test data for MemoryStream");
                memoryStream.Write(sampleData, 0, sampleData.Length);
                Console.WriteLine($"Data written. New length: {memoryStream.Length}");

                // Restablece la posición para una posible lectura
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

### Ver también

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


