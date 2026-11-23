---
title: "DigitalSignatureCollection.GetEnumerator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode DigitalSignatureCollection. Obtenez l'énumérateur pour DigitalSignatureCollection, cet énumérateur permet d'itérer sur la collection"
type: docs
url: /fr/net/aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/
---
## DigitalSignatureCollection.GetEnumerator method

Obtenez l'énumérateur pour DigitalSignatureCollection, cet énumérateur permet d'itérer sur la collection

```csharp
public IEnumerator GetEnumerator()
```

### Valeur de retour

L'énumérateur pour l'itération.

### Exemples

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
            // Créez une nouvelle collection de signatures numériques
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();

            // Créez des signatures numériques d'exemple avec les paramètres requis
            DigitalSignature signature1 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 1", DateTime.Now);
            DigitalSignature signature2 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 2", DateTime.Now);

            // Ajoutez des signatures à la collection
            signatures.Add(signature1);
            signatures.Add(signature2);

            try
            {
                // Obtenez l'énumérateur
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

### Voir aussi

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


