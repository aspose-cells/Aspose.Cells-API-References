---
title: "DigitalSignatureCollection.GetEnumerator"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignatureCollection yöntemi. DigitalSignatureCollection için yineleyiciyi alın; bu yineleyici koleksiyon üzerinde iterasyona izin verir."
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/
---
## DigitalSignatureCollection.GetEnumerator method

DigitalSignatureCollection için enumeratörü alın, bu enumeratör koleksiyon üzerinde yineleme yapmayı sağlar.

```csharp
public IEnumerator GetEnumerator()
```

### Dönüş Değeri

İterasyon için yineleyici.

### Örnekler

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
            // Yeni bir dijital imza koleksiyonu oluşturun
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();

            // Gerekli parametrelerle örnek dijital imzalar oluşturun
            DigitalSignature signature1 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 1", DateTime.Now);
            DigitalSignature signature2 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 2", DateTime.Now);

            // İmzaları koleksiyona ekleyin
            signatures.Add(signature1);
            signatures.Add(signature2);

            try
            {
                // Yineleyiciyi alın
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

### Ayrıca Bakınız

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


