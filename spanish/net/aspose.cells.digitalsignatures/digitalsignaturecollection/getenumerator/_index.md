---
title: "DigitalSignatureCollection.GetEnumerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método DigitalSignatureCollection. Obtén el enumerador para DigitalSignatureCollection; este enumerador permite iterar sobre la colección"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/
---
## DigitalSignatureCollection.GetEnumerator method

Obtener el enumerador para DigitalSignatureCollection, este enumerador permite iterar sobre la colección

```csharp
public IEnumerator GetEnumerator()
```

### Valor de retorno

El enumerador para iterar.

### Ejemplos

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
            // Crear una nueva colección de firmas digitales
            DigitalSignatureCollection signatures = new DigitalSignatureCollection();

            // Crear firmas digitales de ejemplo con los parámetros requeridos
            DigitalSignature signature1 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 1", DateTime.Now);
            DigitalSignature signature2 = new DigitalSignature(
                new X509Certificate2(), "Sample comment 2", DateTime.Now);

            // Agregar firmas a la colección
            signatures.Add(signature1);
            signatures.Add(signature2);

            try
            {
                // Obtener el enumerador
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

### Ver también

* class [DigitalSignatureCollection](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


