---
title: "DigitalSignature.Certificate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DigitalSignature. Объект сертификата, использованный для подписи документа"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/certificate/
---
## DigitalSignature.Certificate property

Объект сертификата, использованный для подписи документа.

```csharp
public X509Certificate2 Certificate { get; set; }
```

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Создать сертификат (в реальном сценарии вы бы загрузили реальный сертификат)
            // Это только для демонстрации — не будет действительным для реального подписания
            X509Certificate2 certificate = new X509Certificate2();
            
            // Создать цифровую подпись с сертификатом
            DigitalSignature signature = new DigitalSignature(
                certificate, 
                "Test signature", 
                DateTime.Now);
            
            // Отобразить текущую информацию о сертификате
            Console.WriteLine("Current Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("Current Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Создайте коллекцию и добавьте в неё подпись
            DigitalSignatureCollection signatureCollection = new DigitalSignatureCollection();
            signatureCollection.Add(signature);
            
            // Добавьте подписи в книгу
            workbook.AddDigitalSignature(signatureCollection);
            
            // Создайте новый сертификат (симулированный)
            X509Certificate2 newCertificate = new X509Certificate2();
            
            // Измените свойство сертификата
            signature.Certificate = newCertificate;
            
            // Отобразите информацию о новом сертификате
            Console.WriteLine("New Certificate Subject: " + signature.Certificate.Subject);
            Console.WriteLine("New Certificate Issuer: " + signature.Certificate.Issuer);
            
            // Сохраните книгу с цифровой подписью
            workbook.Save("DigitalSignatureWithCertificate.xlsx");
        }
    }
}
```

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


