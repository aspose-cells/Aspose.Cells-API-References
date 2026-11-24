---
title: "CustomImplementationFactory.CreateMemoryStream"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CustomImplementationFactory-Methode. Erstellt eine Instanz von MemoryStream oder einer benutzerdefinierten Implementierung von MemoryStream"
type: docs
url: /de/net/aspose.cells/customimplementationfactory/creatememorystream/
---
## CreateMemoryStream() {#creatememorystream}

Erstellen Sie eine Instanz von MemoryStream oder einer benutzerdefinierten Implementierung von MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream()
```

### Rückgabewert

Die MemoryStream-Instanz.

### Beispiele

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
                // Erstellen Sie eine Instanz von CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Demonstriere CreateMemoryStream ohne Parameter
                MemoryStream stream1 = factory.CreateMemoryStream();
                Console.WriteLine($"MemoryStream created with default capacity. Length: {stream1.Length}");

                // Demonstriere CreateMemoryStream mit Kapazitätsparameter
                int capacity = 2048;
                MemoryStream stream2 = factory.CreateMemoryStream(capacity);
                Console.WriteLine($"MemoryStream created with capacity: {capacity}. Length: {stream2.Length}");

                // Schreibe einige Daten, um die Funktionalität zu demonstrieren
                byte[] data = System.Text.Encoding.UTF8.GetBytes("Sample data for MemoryStream");
                stream2.Write(data, 0, data.Length);
                Console.WriteLine($"Data written to MemoryStream. New length: {stream2.Length}");

                // Setze die Position zurück für mögliches Lesen
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

### Siehe auch

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateMemoryStream(int) {#creatememorystream_1}

Erstellen Sie eine Instanz von MemoryStream oder einer benutzerdefinierten Implementierung von MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream(int capacity)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Kapazität | Int32 | Anfängliche Kapazität für den MemoryStream |

### Rückgabewert

Die MemoryStream-Instanz.

### Beispiele

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
                // Erstellen Sie eine Instanz von CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Rufe CreateMemoryStream mit einem Kapazitätsparameter auf
                int capacity = 4096;
                MemoryStream memoryStream = factory.CreateMemoryStream(capacity);

                // Zeige Informationen über den erstellten MemoryStream an
                Console.WriteLine($"MemoryStream created successfully with capacity: {capacity}");
                Console.WriteLine($"Initial length: {memoryStream.Length}");
                Console.WriteLine($"Initial capacity: {memoryStream.Capacity}");

                // Schreibe Beispieldaten, um die Funktionalität zu demonstrieren
                byte[] sampleData = System.Text.Encoding.UTF8.GetBytes("Test data for MemoryStream");
                memoryStream.Write(sampleData, 0, sampleData.Length);
                Console.WriteLine($"Data written. New length: {memoryStream.Length}");

                // Setze die Position zurück für mögliches Lesen
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

### Siehe auch

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


