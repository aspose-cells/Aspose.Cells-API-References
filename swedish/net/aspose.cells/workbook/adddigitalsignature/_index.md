---
title: "Workbook.AddDigitalSignature"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Lägger till digital signatur i en OOXML-kalkylbladsfil Excel2007 och senare"
type: docs
url: /sv/net/aspose.cells/workbook/adddigitalsignature/
---
## Workbook.AddDigitalSignature method

Lägger till digital signatur i en OOXML-kalkylbladsfil (Excel2007 och senare).

```csharp
public void AddDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| digitalSignatureCollection | DigitalSignatureCollection |  |

### Anmärkningar

Stöder endast att lägga till Xmldsig Digital Signature till en OOXML-kalkylbladsfil

### Exempel

```csharp
using System;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;

namespace AsposeCellsExamples
{
    public class WorkbookMethodAddDigitalSignatureWithDigitalSignatureCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite exempeldata
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Digital Signature");

            // Läs in certifikat (byt ut mot din egen certifikatväg och lösenord)
            X509Certificate2 certificate = new X509Certificate2("DrWatson.pfx", "1234567890");

            // Skapa digital signatur
            DigitalSignature digitalSignature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);

            // Skapa digital signatursamling och lägg till signatur
            DigitalSignatureCollection digitalSignatureCollection = new DigitalSignatureCollection();
            digitalSignatureCollection.Add(digitalSignature);

            // Lägg till digital signatur till arbetsboken
            workbook.AddDigitalSignature(digitalSignatureCollection);

            // Spara arbetsboken
            workbook.Save("DigitallySignedWorkbook.xlsx");
        }
    }
}
```

### Se även

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


