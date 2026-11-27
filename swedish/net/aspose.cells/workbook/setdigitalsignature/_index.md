---
title: "Workbook.SetDigitalSignature"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Ställer in digital signatur för en kalkylbladsfil Excel2007 och senare"
type: docs
url: /sv/net/aspose.cells/workbook/setdigitalsignature/
---
## Workbook.SetDigitalSignature method

Ställer in digital signatur för ett kalkylarksfil (Excel2007 och senare).

```csharp
public void SetDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Anmärkningar

Stöder endast att lägga till Xmldsig Digital Signature

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Sökväg till källkatalog
            string sourceDir = "SourceDirectory/";
            
            // Sökväg till utdatakatalog
            string outputDir = "OutputDirectory/";

            // Läs in arbetsboken
            Workbook workbook = new Workbook(sourceDir + "TestCert.xlsx");

            // Skapa digital signatursamling
            DigitalSignatureCollection digitalSignatures = new DigitalSignatureCollection();

            // Läs in certifikatfil
            string certPath = sourceDir + "certs\\sample.pfx";
            byte[] certData = File.ReadAllBytes(certPath);

            // Skapa digital signatur
            DigitalSignature signature = new DigitalSignature(certData, "1234567890", "Sample Signer", DateTime.Now);

            // Lägg till signatur i samlingen
            digitalSignatures.Add(signature);

            // Ställ in digital signatur för workbook
            workbook.SetDigitalSignature(digitalSignatures);

            // Spara arbetsboken
            workbook.Save(outputDir + "DigitallySignedWorkbook.xlsx");

            Console.WriteLine("Digital signature set successfully.");
        }
    }
}
```

### Se även

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


