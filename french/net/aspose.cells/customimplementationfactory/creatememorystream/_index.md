---
title: "CustomImplementationFactory.CreateMemoryStream"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CustomImplementationFactory. Créez une instance de MemoryStream ou une implémentation personnalisée de MemoryStream"
type: docs
url: /fr/net/aspose.cells/customimplementationfactory/creatememorystream/
---
## CreateMemoryStream() {#creatememorystream}

Créez une instance de MemoryStream ou d'une implémentation personnalisée de MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream()
```

### Valeur de retour

L'instance MemoryStream.

### Exemples

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
                // Créez une instance de CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Démontrez CreateMemoryStream sans paramètres
                MemoryStream stream1 = factory.CreateMemoryStream();
                Console.WriteLine($"MemoryStream created with default capacity. Length: {stream1.Length}");

                // Démontrez CreateMemoryStream avec le paramètre de capacité
                int capacity = 2048;
                MemoryStream stream2 = factory.CreateMemoryStream(capacity);
                Console.WriteLine($"MemoryStream created with capacity: {capacity}. Length: {stream2.Length}");

                // Écrivez des données pour démontrer la fonctionnalité
                byte[] data = System.Text.Encoding.UTF8.GetBytes("Sample data for MemoryStream");
                stream2.Write(data, 0, data.Length);
                Console.WriteLine($"Data written to MemoryStream. New length: {stream2.Length}");

                // Réinitialisez la position pour une éventuelle lecture
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

### Voir aussi

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateMemoryStream(int) {#creatememorystream_1}

Créez une instance de MemoryStream ou d'une implémentation personnalisée de MemoryStream.

```csharp
public virtual MemoryStream CreateMemoryStream(int capacity)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| capacité | Int32 | Capacité initiale pour le MemoryStream |

### Valeur de retour

L'instance MemoryStream.

### Exemples

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
                // Créez une instance de CustomImplementationFactory
                CustomImplementationFactory factory = new CustomImplementationFactory();

                // Appelez CreateMemoryStream avec un paramètre de capacité
                int capacity = 4096;
                MemoryStream memoryStream = factory.CreateMemoryStream(capacity);

                // Affichez les informations sur le MemoryStream créé
                Console.WriteLine($"MemoryStream created successfully with capacity: {capacity}");
                Console.WriteLine($"Initial length: {memoryStream.Length}");
                Console.WriteLine($"Initial capacity: {memoryStream.Capacity}");

                // Écrivez des données d'exemple pour démontrer le fonctionnement
                byte[] sampleData = System.Text.Encoding.UTF8.GetBytes("Test data for MemoryStream");
                memoryStream.Write(sampleData, 0, sampleData.Length);
                Console.WriteLine($"Data written. New length: {memoryStream.Length}");

                // Réinitialisez la position pour une éventuelle lecture
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

### Voir aussi

* class [CustomImplementationFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


