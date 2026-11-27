---
title: "DigitalSignature.Image"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DigitalSignature-egenskap. Anger en bild för den digitala signaturen. Standardvärdet är null"
type: docs
url: /sv/net/aspose.cells.digitalsignatures/digitalsignature/image/
---
## DigitalSignature.Image property

Anger en bild för den digitala signaturen. Standardvärdet är null.

```csharp
public byte[] Image { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.DigitalSignatures;
using System.Security.Cryptography.X509Certificates;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyImageDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Lägg till en signaturlinje i kalkylbladet
            Picture picture = ws.Pictures[0];
            SignatureLine signatureLine = picture.SignatureLine;
            signatureLine.Signer = "Test Signer";
            signatureLine.Title = "Test Title";

            // Skapa ett testcertifikat (vid verklig användning, läs in från fil)
            byte[] certData = new byte[0]; // Replace with actual certificate bytes
            X509Certificate2 certificate = new X509Certificate2(certData);

            // Skapa digital signatur med bild
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            signature.Image = File.ReadAllBytes("signature.png"); // Replace with actual image path

            // Lägg till signatur och spara
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            // Spara till minnesström
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


