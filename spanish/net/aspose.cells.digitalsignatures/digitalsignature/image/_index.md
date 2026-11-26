---
title: "DigitalSignature.Image"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DigitalSignature. Especifica una imagen para la firma digital. El valor predeterminado es null"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/image/
---
## DigitalSignature.Image property

Especifica una imagen para la firma digital. El valor predeterminado es null.

```csharp
public byte[] Image { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Agregar una línea de firma a la hoja de cálculo
            Picture picture = ws.Pictures[0];
            SignatureLine signatureLine = picture.SignatureLine;
            signatureLine.Signer = "Test Signer";
            signatureLine.Title = "Test Title";

            // Crear un certificado de prueba (en uso real, cargar desde archivo)
            byte[] certData = new byte[0]; // Replace with actual certificate bytes
            X509Certificate2 certificate = new X509Certificate2(certData);

            // Crear firma digital con imagen
            DigitalSignature signature = new DigitalSignature(certificate, "Test Signature", DateTime.Now);
            signature.Image = File.ReadAllBytes("signature.png"); // Replace with actual image path

            // Agregar firma y guardar
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            // Guardar en flujo de memoria
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


