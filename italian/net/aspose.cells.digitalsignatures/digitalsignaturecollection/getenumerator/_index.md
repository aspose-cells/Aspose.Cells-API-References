---
title: "DigitalSignatureCollection.GetEnumerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo DigitalSignatureCollection. Ottieni l'enumeratore per DigitalSignatureCollection; questo enumeratore consente l'iterazione sulla collezione"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/
---
## DigitalSignatureCollection.GetEnumerator method

Ottieni l'enumeratore per DigitalSignatureCollection, questo enumeratore consente l'iterazione sulla collezione

```csharp
public IEnumerator GetEnumerator()
```

### Valore di ritorno

L'enumeratore per l'iterazione.

### Esempi

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
            // Crea una nuova collezione di firme digitali
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();

            // Crea firme digitali di esempio con i parametri richiesti
            DigitalSignature signature1 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 1", DateTime.Now);
            DigitalSignature signature2 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 2", DateTime.Now);

            // Aggiungi firme alla collezione
            signatures.Add(signature1);
            signatures.Add(signature2);

            try
            {
                // Ottieni l'enumeratore
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

### Vedi anche

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


