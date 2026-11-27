---
title: "Klass DigitalSignatureCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DigitalSignatures.DigitalSignatureCollection klass. Tillhandahåller en samling av digitala signaturer som är bifogade till ett dokument"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class

Tillhandahåller en samling digitala signaturer som är bifogade till ett dokument.

```csharp
public class DigitalSignatureCollection : IEnumerable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | Konstruktorn för DigitalSignatureCollection. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | Lägg till en signatur i DigitalSignatureCollection. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | Hämta enumeratorn för DigitalSignatureCollection, den här enumeratorn möjliggör iteration över samlingen |

### Exempel

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
            // Läs in en arbetsbok från en signerad källfil
            Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");

            // Kontrollera om arbetsboken är digitalt signerad
            Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);

            // Hämta den digitala signatursamlingen från arbetsboken
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // Iterera över de digitala signaturerna i samlingen
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine("Comments: " + existingDs.Comments);
                    Console.WriteLine("Sign Time: " + existingDs.SignTime);
                    Console.WriteLine("Is Valid: " + existingDs.IsValid);
                }

                // Skapa en ny digital signatur
                X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
                DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);

                // Lägg till den nya digitala signaturen i samlingen
                existingDsc.Add(newSignature);
            }     
            

            // Spara arbetsboken med den nya digitala signaturen
            signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
            signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


