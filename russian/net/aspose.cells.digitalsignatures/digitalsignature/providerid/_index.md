---
title: "DigitalSignature.ProviderId"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DigitalSignature. Указывает идентификатор класса поставщика подписи. Значение по умолчанию — пустой GUID, состоящий только из нулей"
type: docs
url: /ru/net/aspose.cells.digitalsignatures/digitalsignature/providerid/
---
## DigitalSignature.ProviderId property

Указывает идентификатор класса поставщика подписи. Значение по умолчанию — Empty (все нули) Guid.

```csharp
public Guid ProviderId { get; set; }
```

### Примечания

Криптографический сервисный провайдер (CSP) — это независимый программный модуль, который фактически выполняет криптографические алгоритмы для аутентификации, кодирования и шифрования. Microsoft Office резервирует значение {00000000-0000-0000-0000-000000000000} для своего провайдера подписи по умолчанию и {000CD6A4-0000-0000-C000-000000000046} для провайдера подписи восточноазиатского региона. GUID дополнительно установленного провайдера следует получить из документации, поставляемой с провайдером.

### Примеры

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
            // Создать самоподписанный сертификат
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

            // Создать книгу и добавить строку подписи
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Добавить заглушку‑изображение с линией подписи
            using (var ms = new MemoryStream())
            {
                ms.Write(new byte[] { 0x42, 0x4D, 0x1E, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x1A, 0x00, 0x00, 0x00 }, 0, 14);
                ms.Position = 0;
                
                int idx = ws.Pictures.Add(0, 0, ms);
                Picture pic = ws.Pictures[idx];
                pic.SignatureLine = new SignatureLine();
                pic.SignatureLine.ProviderId = Guid.NewGuid();
            }

            // Создать цифровую подпись
            var signature = new DigitalSignature(certificate, "Aspose ProviderId Demo", DateTime.Now);
            signature.ProviderId = ws.Pictures[0].SignatureLine.ProviderId;

            // Установить цифровую подпись и сохранить
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

### См. также

* class [DigitalSignature](../)
* namespace [Aspose.Cells.DigitalSignatures](../../../aspose.cells.digitalsignatures/)
* assembly [Aspose.Cells](../../../)


