---
title: "Klasse DigitalSignatureCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DigitalSignatures.DigitalSignatureCollection Klasse. Stellt eine Sammlung digitaler Signaturen bereit, die an ein Dokument angehängt sind"
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class

Stellt eine Sammlung digitaler Signaturen bereit, die an ein Dokument angehängt sind.

```csharp
public class DigitalSignatureCollection : IEnumerable
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | Der Konstruktor von DigitalSignatureCollection. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | Füge eine Signatur zu DigitalSignatureCollection hinzu. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | Hole den Enumerator für DigitalSignatureCollection, dieser Enumerator ermöglicht die Iteration über die Sammlung |

### Beispiele

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
            // Lade eine Arbeitsmappe aus einer signierten Quelldatei
            Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");

            // Prüfen, ob die Arbeitsmappe digital signiert ist
            Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);

            // Hole die digitale Signaturensammlung aus der Arbeitsmappe
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // Iteriere über die digitalen Signaturen in der Sammlung
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine("Comments: " + existingDs.Comments);
                    Console.WriteLine("Sign Time: " + existingDs.SignTime);
                    Console.WriteLine("Is Valid: " + existingDs.IsValid);
                }

                // Erstelle eine neue digitale Signatur
                X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
                DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);

                // Füge die neue digitale Signatur zur Sammlung hinzu
                existingDsc.Add(newSignature);
            }     
            

            // Speichern Sie die Arbeitsmappe mit der neuen digitalen Signatur
            signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
            signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


