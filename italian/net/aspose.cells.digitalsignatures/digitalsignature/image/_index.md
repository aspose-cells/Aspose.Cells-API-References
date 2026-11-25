---
title: "DigitalSignature.Image"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DigitalSignature. Specifica un'immagine per la firma digitale. Il valore predefinito è null"
type: docs
url: /it/net/aspose.cells.digitalsignatures/digitalsignature/image/
---
## DigitalSignature.Image property

Specifica un'immagine per la firma digitale. Il valore predefinito è null.

```csharp
public byte[] Image { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Aggiungi una linea di firma al foglio di lavoro
            Picture picture = ws.Pictures[0];
            SignatureLine signatureLine = picture.SignatureLine;
            signatureLine.Signer = "Test Signer";
            signatureLine.Title = "Test Title";

            // Crea un certificato di test (in un utilizzo reale, carica da file)
            byte[] certData = new byte[0]; // Replace with actual certificate bytes
            X509Certificate2 certificate = new X509Certificate2(certData);

            // Crea una firma digitale con immagine
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            signature.Image = File.ReadAllBytes("signature.png"); // Replace with actual image path

            // Aggiungi la firma e salva
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            // Salva su stream di memoria
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


