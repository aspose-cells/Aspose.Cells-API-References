---
title: "DigitalSignature.Certificate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DigitalSignature özelliği. Belgeyi imzalamak için kullanılan sertifika nesnesi"
type: docs
url: /tr/net/aspose.cells.digitalsignatures/digitalsignature/certificate/
---
## DigitalSignature.Certificate property

Belgeyi imzalamak için kullanılan sertifika nesnesi.

```csharp
public X509Certificate2 Certificate { get; set; }
```

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir sertifika oluştur (gerçek senaryoda, gerçek bir sertifika yüklersiniz)
            // Bu sadece gösterim amaçlıdır - gerçek imzalama için geçerli olmayacaktır
            X509Certificate2 certificate = new X509Certificate2();
            
            // Sertifika ile bir dijital imza oluştur
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Test signature", 
                DateTime.Now);
            
            // Mevcut sertifika bilgilerini göster
            Console.WriteLine("Current Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("Current Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Bir koleksiyon oluşturun ve imzayı ona ekleyin
            DigitalSignatureCollection signatureCollection = new DigitalSignatureCollection();
            signatureCollection.Add(signature);
            
            // İmzaları çalışma kitabına ekleyin
            workbook.AddDigitalSignature(signatureCollection);
            
            // Yeni bir sertifika oluşturun (simüle edilmiş)
            X509Certificate2 newCertificate = new X509Certificate2();
            
            // Sertifika özelliğini değiştirin
            signature.Certificate = newCertificate;
            
            // Yeni sertifika bilgilerini gösterin
            Console.WriteLine("New Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("New Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Çalışma kitabını dijital imza ile kaydedin
            workbook.Save("DigitalSignatureWithCertificate.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


