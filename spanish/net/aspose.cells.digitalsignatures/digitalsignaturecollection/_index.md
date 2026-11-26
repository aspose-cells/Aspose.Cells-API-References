---
title: "Clase DigitalSignatureCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.DigitalSignatures.DigitalSignatureCollection. Proporciona una colección de firmas digitales adjuntas a un documento"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class

Proporciona una colección de firmas digitales adjuntas a un documento.

```csharp
public class DigitalSignatureCollection : IEnumerable
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | El constructor de DigitalSignatureCollection. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | Agregar una firma a DigitalSignatureCollection. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | Obtener el enumerador para DigitalSignatureCollection, este enumerador permite iterar sobre la colección |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignatureCollectionDemo
    {
        public static void DigitalSignatureCollectionExample()
        {
            // Cargar un libro de trabajo desde un archivo fuente firmado
            Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");

            // Verificar si el libro de trabajo está firmado digitalmente
            Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);

            // Obtener la colección de firmas digitales del libro de trabajo
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // Iterar sobre las firmas digitales en la colección
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine("Comments: " + existingDs.Comments);
                    Console.WriteLine("Sign Time: " + existingDs.SignTime);
                    Console.WriteLine("Is Valid: " + existingDs.IsValid);
                }

                // Crear una nueva firma digital
                X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
                DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);

                // Agregar la nueva firma digital a la colección
                existingDsc.Add(newSignature);
            }     
            

            // Guardar el libro de trabajo con la nueva firma digital
            signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
            signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


