---
title: "DigitalSignature.Image"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DigitalSignature-Eigenschaft. Gibt ein Bild für die digitale Signatur an. Standardwert ist null"
type: docs
url: /de/net/aspose.cells.digitalsignatures/digitalsignature/image/
---
## DigitalSignature.Image property

Gibt ein Bild für die digitale Signatur an. Standardwert ist null.

```csharp
public byte[] Image { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Füge eine Signaturzeile zum Arbeitsblatt hinzu
            Picture picture = ws.Pictures[0];
            SignatureLine signatureLine = picture.SignatureLine;
            signatureLine.Signer = "Test Signer";
            signatureLine.Title = "Test Title";

            // Erstelle ein Testzertifikat (bei realer Verwendung aus Datei laden)
            byte[] certData = new byte[0]; // Replace with actual certificate bytes
            X509Certificate2 certificate = new X509Certificate2(certData);

            // Erstelle digitale Signatur mit Bild
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            signature.Image = File.ReadAllBytes("signature.png"); // Replace with actual image path

            // Füge Signatur hinzu und speichere
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            // In den Speicherstream speichern
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


