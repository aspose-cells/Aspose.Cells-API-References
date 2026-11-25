---
title: "Class DigitalSignatureCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.DigitalSignatures.DigitalSignatureCollection. Fornisce una collezione di firme digitali allegate a un documento"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignaturecollection/
---
## DigitalSignatureCollection class

Fornisce una raccolta di firme digitali allegate a un documento.

```csharp
public class DigitalSignatureCollection : IEnumerable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DigitalSignatureCollection](digitalsignaturecollection/)() | Il costruttore di DigitalSignatureCollection. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.digitalsignatures/digitalsignaturecollection/add/)(DigitalSignature) | Aggiungi una firma a DigitalSignatureCollection. |
| [GetEnumerator](../../aspose.cells.digitalsignatures/digitalsignaturecollection/getenumerator/)() | Ottieni l'enumeratore per DigitalSignatureCollection, questo enumeratore consente l'iterazione sulla collezione |

### Esempi

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
            // Carica una cartella di lavoro da un file di origine firmato
            Workbook signedWorkbook = new Workbook(@"DigitalSignatureCollection_original.xlsx");

            // Verifica se la cartella di lavoro è firmata digitalmente
            Console.WriteLine("Is the workbook digitally signed? " + signedWorkbook.IsDigitallySigned);

            // Ottieni la collezione di firme digitali dalla cartella di lavoro
            DigitalSignatureCollection existingDsc = signedWorkbook.GetDigitalSignature();

            if (existingDsc != null)
            {
                // Itera sulle firme digitali nella collezione
                foreach (DigitalSignature existingDs in existingDsc)
                {
                    Console.WriteLine("Comments: " + existingDs.Comments);
                    Console.WriteLine("Sign Time: " + existingDs.SignTime);
                    Console.WriteLine("Is Valid: " + existingDs.IsValid);
                }

                // Crea una nuova firma digitale
                X509Certificate2 certificate = new X509Certificate2("path_to_certificate.pfx", "password");
                DigitalSignature newSignature = new DigitalSignature(certificate, "New signature comment", DateTime.Now);

                // Aggiungi la nuova firma digitale alla collezione
                existingDsc.Add(newSignature);
            }     
            

            // Salva la cartella di lavoro con la nuova firma digitale
            signedWorkbook.Save("DigitalSignatureCollectionExample.xlsx");
            signedWorkbook.Save("DigitalSignatureCollectionExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.DigitalSignatures](../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../)


