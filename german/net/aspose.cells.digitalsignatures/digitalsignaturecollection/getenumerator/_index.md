---
title: "DigitalSignatureCollection.GetEnumerator"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignatureCollection-Methode. Hole den Enumerator für DigitalSignatureCollection; dieser Enumerator ermöglicht die Iteration über die Sammlung"
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/
---
## DigitalSignatureCollection.GetEnumerator method

Hole den Enumerator für DigitalSignatureCollection, dieser Enumerator ermöglicht die Iteration über die Sammlung

```csharp
public IEnumerator GetEnumerator()
```

### Rückgabewert

Der Enumerator zur Iteration.

### Beispiele

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
            // Erstelle eine neue digitale Signatursammlung
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();

            // Erstelle Beispiel-Digitalsignaturen mit den erforderlichen Parametern
            DigitalSignature signature1 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 1", DateTime.Now);
            DigitalSignature signature2 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 2", DateTime.Now);

            // Füge Signaturen zur Sammlung hinzu
            signatures.Add(signature1);
            signatures.Add(signature2);

            try
            {
                // Hole den Enumerator
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

### Siehe auch

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


