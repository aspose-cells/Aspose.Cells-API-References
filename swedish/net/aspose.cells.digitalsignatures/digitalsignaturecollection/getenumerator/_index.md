---
title: "DigitalSignatureCollection.GetEnumerator"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignatureCollection-metod. Hämta enumeratorn för DigitalSignatureCollection; denna enumerator möjliggör iteration över samlingen"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/
---
## DigitalSignatureCollection.GetEnumerator method

Hämta enumeratorn för DigitalSignatureCollection, den här enumeratorn möjliggör iteration över samlingen

```csharp
public IEnumerator GetEnumerator()
```

### Returvärde

Enumeratorn för iteration.

### Exempel

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
            // Skapa en ny digital signatursamling
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();

            // Skapa exempel på digitala signaturer med nödvändiga parametrar
            DigitalSignature signature1 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 1", DateTime.Now);
            DigitalSignature signature2 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 2", DateTime.Now);

            // Lägg till signaturer i samlingen
            signatures.Add(signature1);
            signatures.Add(signature2);

            try
            {
                // Hämta enumeratorn
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

### Se även

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


