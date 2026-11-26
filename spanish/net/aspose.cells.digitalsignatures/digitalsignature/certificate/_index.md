---
title: "DigitalSignature.Certificate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DigitalSignature. Objeto Certificate que se utilizó para firmar el documento"
type: docs
url: /es/net/aspose.cells.digitalsignatures/digitalsignature/certificate/
---
## DigitalSignature.Certificate property

Objeto de certificado que se utilizó para firmar el documento.

```csharp
public X509Certificate2 Certificate { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;
    using System.Security.Cryptography.X509Certificates;

    public class DigitalSignaturePropertyCertificateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear un certificado (en un escenario real, cargarías un certificado real)
            // Esto es solo para demostración - no será válido para una firma real
            X509Certificate2 certificate = new X509Certificate2();
            
            // Crear una firma digital con el certificado
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Test signature", 
                DateTime.Now);
            
            // Mostrar información actual del certificado
            Console.WriteLine("Current Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("Current Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Crear una colección y agregar la firma a ella
            DigitalSignatureCollection signatureCollection = new DigitalSignatureCollection();
            signatureCollection.Add(signature);
            
            // Agregar las firmas al libro de trabajo
            workbook.AddDigitalSignature(signatureCollection);
            
            // Crear un nuevo certificado (simulado)
            X509Certificate2 newCertificate = new X509Certificate2();
            
            // Cambiar la propiedad del certificado
            signature.Certificate = newCertificate;
            
            // Mostrar la información del nuevo certificado
            Console.WriteLine("New Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("New Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Guardar el libro de trabajo con firma digital
            workbook.Save("DigitalSignatureWithCertificate.xlsx");
        }
    }
}
```

### Ver también

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


