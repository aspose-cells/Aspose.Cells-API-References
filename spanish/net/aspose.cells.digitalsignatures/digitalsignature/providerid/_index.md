---
title: "DigitalSignature.ProviderId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DigitalSignature. Especifica el ID de clase del proveedor de firmas. El valor predeterminado es Guid vacío con todos ceros"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

Especifica el ID de clase del proveedor de firma. El valor predeterminado es Empty (todos ceros) Guid.

```csharp
public Guid ProviderId { get; set; }
```

### Observaciones

El proveedor de servicios criptográficos (CSP) es un módulo de software independiente que realmente ejecuta algoritmos criptográficos para autenticación, codificación y cifrado. Microsoft Office reserva el valor {00000000-0000-0000-0000-000000000000} para su proveedor de firmas predeterminado, y {000CD6A4-0000-0000-C000-000000000046} para su proveedor de firmas de Asia Oriental. El GUID del proveedor adicionalmente instalado debe obtenerse de la documentación suministrada con el proveedor.

### Ejemplos

```csharp
using System;
using System.IO;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;
using Aspose.Cells;
using Aspose.Cells.DigitalSignatures;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DigitalSignaturePropertyProviderIdDemo
    {
        public static void Run()
        {
            // Crear certificado autofirmado
            X509Certificate2 certificate;
            using (var rsa = RSA.Create())
            {
                var request = new CertificateRequest(
                    new X500DistinguishedName("cn=AsposeTest"),
                    rsa,
                    HashAlgorithmName.SHA256,
                    RSASignaturePadding.Pkcs1);
                
                certificate = request.CreateSelfSigned(DateTimeOffset.Now, DateTimeOffset.Now.AddHours(1));
            }

            // Crear libro de trabajo y agregar línea de firma
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Agregar imagen ficticia con línea de firma
            using (var ms = new MemoryStream())
            {
                ms.Write(new byte[] { 0x42, 0x4D, 0x1E, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x1A, 0x00, 0x00, 0x00 }, 0, 14);
                ms.Position = 0;
                
                int idx = ws.Pictures.Add(0, 0, ms);
                Picture pic = ws.Pictures[idx];
                pic.SignatureLine = new SignatureLine();
                pic.SignatureLine.ProviderId = Guid.NewGuid();
            }

            // Crear firma digital
            var signature = new DigitalSignature(certificate, "Aspose ProviderId Demo", DateTime.Now);
            signature.ProviderId = ws.Pictures[0].SignatureLine.ProviderId;

            // Establecer firma digital y guardar
            DigitalSignatureCollection dsCollection = new DigitalSignatureCollection();
            dsCollection.Add(signature);
            wb.SetDigitalSignature(dsCollection);

            using (MemoryStream output = new MemoryStream())
            {
                wb.Save(output, SaveFormat.Xlsx);
            }
        }
    }
}
```

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


