---
title: "DigitalSignatureCollection.GetEnumerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод DigitalSignatureCollection. Получить перечислитель для DigitalSignatureCollection; этот перечислитель позволяет выполнять итерацию по коллекции"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/
---
## DigitalSignatureCollection.GetEnumerator method

Получить перечислитель для DigitalSignatureCollection, этот перечислитель позволяет выполнять итерацию по коллекции.

```csharp
public IEnumerator GetEnumerator()
```

### Возвращаемое значение

Перечислитель для итерации.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Collections;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignatureCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Создать новую коллекцию цифровых подписей
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();

            // Создать образцы цифровых подписей с необходимыми параметрами
            DigitalSignature signature1 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 1", DateTime.Now);
            DigitalSignature signature2 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 2", DateTime.Now);

            // Добавить подписи в коллекцию
            signatures.Add(signature1);
            signatures.Add(signature2);

            try
            {
                // Получить перечислитель
                IEnumerator enumerator = signatures.GetEnumerator();

                Console.WriteLine("Iterating through digital signatures:");
                int count = 0;
                while (enumerator.MoveNext())
                {
                    DigitalSignature current = (DigitalSignature)enumerator.Current;
                    Console.WriteLine($"Signature #{++count} found");
                }

                Console.WriteLine($"Total signatures: {count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


